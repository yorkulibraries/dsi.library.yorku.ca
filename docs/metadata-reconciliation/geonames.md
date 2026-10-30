---
title: GeoNames Reconciliation Service
icon: lucide/map-pin-search
---

# Using the GeoNames Reconciliation Service with OpenRefine

This guide walks you through reconciling data in [OpenRefine](https://openrefine.org/) against [GeoNames](https://www.geonames.org/), matching strings in your project to geographic entities and retrieving their names, URIs, and coordinates.

---

## Prerequisites

- OpenRefine installed and running
- A project open in OpenRefine with a column you want to reconcile

---

## Step 1: Open the Reconciliation Dialog

1. Click the **arrow** at the top of the column you want to reconcile
2. Choose **Reconcile → Start Reconciling...**

---

## Step 2: Add the GeoNames Reconciliation Service

1. Click **Add Standard Service** in the bottom left corner of the dialog
2. Enter the following URL:
   ```
   https://reconcile.library.yorku.ca/geonames/
   ```
3. Click **Add Service**

The service will appear in the list as **GeoNames Reconciliation Service**.

---

## Step 3: Choose a Reconciliation Type

You will see a list of available geographic entity types. Use **/geonames/all** if you need the broadest search capabilities possible.

---

## Step 4: Start Reconciling

Click **Start Reconciling** in the bottom right corner. OpenRefine will query the GeoNames API for each cell in your column. This may take a moment depending on the size of your project.

---

## Step 5: Review and Accept Matches

Once reconciliation is complete, each cell will display the closest matches found. For each cell:

- Click on a candidate to open the corresponding entry on the GeoNames site and verify it is the correct match
- Click the **single check** (✓) beside a match to accept it for that cell only
- Click the **double check** (✓✓) beside a match to accept it for all cells containing the same value

Repeat until you have accepted or dismissed matches for all cells.

---

## Step 6: Save the Reconciled Data

!!! important
    Although reconciled matches appear in your OpenRefine project, OpenRefine is still storing the original values internally. You must explicitly extract the reconciled data into a new column to ensure it is included when you export your project.

### To add a new column containing the name and coordinates:

1. Click the **arrow** at the top of the reconciled column
2. Choose **Edit Columns → Add column based on this column...**
3. Give the new column an appropriate name — a good convention is the original column name plus a suffix such as `_name`
4. In the [**GREL expression**](https://openrefine.org/docs/manual/grel) box, enter:
   ```
   cell.recon.match.name
   ```
5. Click **OK**

### To add a new column containing the URI:

1. Repeat the steps above
2. Name the column with a suffix such as `_uri`
3. In the [**GREL expression**](https://openrefine.org/docs/manual/grel) box, enter:
   ```
   cell.recon.match.id
   ```
4. Click **OK**

### Useful GREL expressions

| What you want | GREL expression |
|---|---|
| Name and coordinates | `cell.recon.match.name` |
| URI only | `cell.recon.match.id` |
| Coordinates only | `replace(substring(cell.recon.match.name, indexOf(cell.recon.match.name, " \| ")), " \| ", "")` |
| Name, coordinates, and URI separated by \| | `cell.recon.match.name + " \| " + cell.recon.match.id` |

!!! note
    The `cell.recon.match.name` field returns the GeoNames name and coordinates separated by a `|`. If you want to split these into separate columns later, use the Name and coordinates expression first, then use **Edit Column → Split into several columns** with `|` as the separator.

---

## Notes

For guidance on handling no matches, dismissing candidates, re-reconciling a column, and other common questions, see [Reconciliation Tips & Troubleshooting](tips.md).

- If a cell shows **no match**, the reconciliation service found nothing close enough to suggest. You may want to check the spelling or try using **/geonames/all** for a broader search.
- If multiple candidates appear and none are correct, click the **×** to dismiss and leave the cell unmatched.
- You can re-reconcile a column at any time by repeating this process.
