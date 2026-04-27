---
title: YUDL Reconciliation Service
icon: simple/drupal
---

# Using the YUDL Reconciliation Service with OpenRefine

This guide walks you through reconciling data in OpenRefine against the YUDL taxonomy authorities. Matching strings in your data to controlled vocabulary terms and retrieving their Term IDs (TIDs).

---

## Prerequisites

- [OpenRefine](https://openrefine.org/) installed and running
- A project open in OpenRefine with a column you want to reconcile

---

## Step 1: Open the Reconciliation Dialog

1. Click the **arrow** at the top of the column you want to reconcile
2. Choose **Reconcile → Start Reconciling...**

---

## Step 2: Add the YUDL Reconciliation Service

1. Click **Add Standard Service** in the bottom left corner of the dialog
2. Enter the following URL:
   ```
   https://digital.library.yorku.ca/api/reconcile
   ```
3. Click **Add Service**

The service will appear in the list as **YUDL Taxonomy Authorities**.

---

## Step 3: Choose a Reconciliation Type

You will see a list of available vocabulary types:

* Person
* Subject
* Corporate Body
* City
* City Section
* Country
* County
* Family
* Genre
* Geographic Location
* Language
* Physical Form
* Province
* Region
* Resource Types
* Rights
* Tags
* Temporal Subjects

Select the taxonomy that matches the content of your column. For example, if your column contains subject headings, select **Subject**.

---

## Step 4: Start Reconciling

Click **Start Reconciling** in the bottom right corner. OpenRefine will query the YUDL Reconciliation Service for each cell in your column. This may take a moment depending on the size of your project.

---

## Step 5: Review and Accept Matches

Once reconciliation is complete, each cell will display the closest matches found. For each cell:

- Click on a candidate to open the corresponding YUDL authority page in your browser and verify it is the correct match
- Click the **single check** (✓) beside a match to accept it for that cell only
- Click the **double check** (✓✓) beside a match to accept it for all cells containing the same value

Repeat until you have accepted or dismissed matches for all cells.

---

## Step 6: Save the Reconciled Data

!!! important 
    Although reconciled matches appear in your OpenRefine project, OpenRefine is still storing the original values internally. You must explicitly extract the reconciled data into a new column to ensure it is included when you export your project.

### To add a new column containing the TID:

1. Click the **arrow** at the top of the reconciled column
2. Choose **Edit Columns → Add column based on this column...**
3. Give the new column a name — a good convention is the original column name plus `_tid`, for example `field_subject_tid`
4. In the **GREL expression** box, enter:
   ```
   cell.recon.match.id
   ```
5. Click **OK**

### To add a new column containing the matched label:

1. Repeat the steps above
2. Name the column with a `_label` suffix, for example `field_subject_label`
3. In the **GREL expression** box, enter:
   ```
   cell.recon.match.name
   ```
4. Click **OK**

### Other useful GREL expressions

| What you want | GREL expression |
|---|---|
| TID only | `cell.recon.match.id` |
| Matched label | `cell.recon.match.name` |
| Match score (0–100) | `cell.recon.best.score` |
| Whether it was auto-matched | `cell.recon.matched` |

---

## Notes

- If a cell shows **no match**, the reconciliation service found nothing close enough to suggest. You may want to check the spelling or try reconciling against a different vocabulary type.
- If multiple candidates appear and none are correct, click the **×** to dismiss and leave the cell unmatched.
- You can re-reconcile a column at any time by repeating this process.
