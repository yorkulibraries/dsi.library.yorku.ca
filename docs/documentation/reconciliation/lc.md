---
title: LoC Reconciliation Service
icon: lucide/library
---

# Using the LoC Reconciliation Service with OpenRefine

This guide walks you through reconciling data in [OpenRefine](https://openrefine.org/) against [Library of Congress authorities](https://id.loc.gov/), matching strings in your project to controlled vocabulary terms and retrieving their labels and URIs.

---

## Prerequisites

- OpenRefine installed and running
- A project open in OpenRefine with a column you want to reconcile

---

## Step 1: Open the Reconciliation Dialog

1. Click the **arrow** at the top of the column you want to reconcile
2. Choose **Reconcile → Start Reconciling...**

---

## Step 2: Add the LoC Reconciliation Service

1. Click **Add Standard Service** in the bottom left corner of the dialog
2. Enter the following URL:
   ```
   http://lc.oceanmeat.tech
   ```
3. Click **Add Service**

The service will appear in the list as **LC Reconciliation Service**.

---

## Step 3: Choose a Reconciliation Type

You will see a list of available vocabulary types. Use **/LoC** if you want to search LCNAF and LCSH together.

---

## Step 4: Start Reconciling

Click **Start Reconciling** in the bottom right corner. OpenRefine will query the LoC Reconciliation Service for each cell in your column. This may take a moment depending on the size of your project.

---

## Step 5: Review and Accept Matches

Once reconciliation is complete, each cell will display the closest matches found. For each cell:

- Click on a candidate to open the corresponding authority page on id.loc.gov and verify it is the correct match
- Click the **single check** (✓) beside a match to accept it for that cell only
- Click the **double check** (✓✓) beside a match to accept it for all cells containing the same value

Repeat until you have accepted or dismissed matches for all cells.

---

## Step 6: Save the Reconciled Data

!!! important
    Although reconciled matches appear in your OpenRefine project, OpenRefine is still storing the original values internally. You must explicitly extract the reconciled data into a new column to ensure it is included when you export your project.

1. Click the **arrow** at the top of the reconciled column
2. Choose **Edit Columns → Add column based on this column...**
3. Give the new column an appropriate name
4. In the **GREL expression** box, enter one of the following depending on what you want to capture:
5. Click **OK**

### Useful GREL expressions

| What you want | GREL expression |
|---|---|
| Label only | `cell.recon.match.name` |
| URI only | `cell.recon.match.id` |
| Label and URI separated by \| | `cell.recon.match.name + " \| " + cell.recon.match.id` |


!!! note
    The label and URI combined option (separated by `|`) is useful if you want to split the column into two later, one for the label, and one for the URI.

---

## Notes

- If a cell shows **no match**, the reconciliation service found nothing close enough to suggest. You may want to check the spelling or try reconciling against a different vocabulary type.
- If multiple candidates appear and none are correct, click the **×** to dismiss and leave the cell unmatched.
- You can re-reconcile a column at any time by repeating this process.
