---
title: Reconciliation Tips & Troubleshooting
icon: lucide/lightbulb
---

# Reconciliation Tips & Troubleshooting

This page collects tips that apply to all three reconciliation services ([YUDL](yudl.md), [LoC](lc.md), and [GeoNames](geonames.md)). The individual guides cover each service in detail; this page covers common questions and problems shared across all of them.

---

## Reviewing and accepting matches

- If a cell shows **no match**, the reconciliation service found nothing close enough to suggest. Check the spelling, try a different vocabulary type (see each guide's Step 3), or consider removing extra text from the value before reconciling.
- If multiple candidates appear and none are correct, click the **×** to dismiss and leave the cell unmatched.
- Click a candidate to open its authority page (YUDL, id.loc.gov, or geonames.org) in your browser to verify it is the correct match.

---

## Reconciling the same column again

OpenRefine lets you re-reconcile a column at any time. Generally you will want to:

1. Click the **arrow** at the top of the column
2. Choose **Reconcile → Start Reconciling...** again
3. Re-add or re-select the service and type, then run the reconciliation again

Re-running reconciliation replaces the existing matches with the new results, so only re-reconcile a column before you have extracted the identifiers into new columns.

---

## Extracting reconciled data

!!! important
    Reconciled matches appear in your project, but OpenRefine **still stores the original values internally**. You must explicitly extract the reconciled data into new columns (see Step 6 in each guide) or it will be lost on export.

- Use [GREL expressions](https://openrefine.org/docs/manual/grel) such as `cell.recon.match.id` and `cell.recon.match.name` to pull the identifier and label into new columns.
- A good naming convention is the original column name plus a suffix (`_tid`, `_label`, `_uri`), so you can tell which columns hold the reconciled values.

---

## Combining two values into one column, then splitting later

If you want both the label and the identifier in a single column, combine them with a `|` separator, e.g.:

```
cell.recon.match.name + " | " + cell.recon.match.id
```

This is useful when you want to capture both values in one step. To separate them afterwards:

1. Click the **arrow** on the combined column
2. Choose **Edit Column → Split into several columns...**
3. Use `|` as the separator

---

## Working with no matches in bulk

If a large number of cells come back unmatched, it is often a sign the values were too messy for the service to match directly. Common fixes:

- **Clean the data first**: trim whitespace, remove punctuation, or drop parenthetical notes from the values.
- **Try a broader type**: for example, GeoNames **/geonames/all** searches more entity types.
- **Manual reconciliation**: for a manageable number of stragglers, search the authority site directly and reconcile the cell by hand.

---

## Something not working?

- Confirm OpenRefine is **running** and that you added the service URL exactly as shown in the relevant guide.
- The reconciliation services are DSI infrastructure. If a service will not load or consistently times out, contact the Digital Scholarship Infrastructure team at [diginit@yorku.ca](mailto:diginit@yorku.ca).
- For questions about OpenRefine itself, see the [OpenRefine documentation](https://openrefine.org/docs) and the [GREL reference](https://openrefine.org/docs/manual/grel).
