---
title: Metadata Reconciliation
icon: lucide/scan-search
---

# Metadata Reconciliation

Metadata reconciliation matches free-text values in your data against controlled vocabularies and authority files, so that your project data links to canonical, persistent identifiers instead of ad hoc strings.

The DSI team runs [OpenRefine](https://openrefine.org/) reconciliation services that return candidate matches for each cell in a column. You review the candidates, accept the correct ones, and extract the identifier (and optionally the label) into new columns for export. All of the guides below follow the same workflow in OpenRefine.

## The services

There are three reconciliation services available. Which one you use depends on the kind of values you are reconciling and the identifiers you want back.

| Service | Guide | Add-service URL | Best for | What you get back | Matches resolve to |
|---|---|---|---|---|---|
| **YUDL** | [YUDL Reconciliation Service](yudl.md) | `https://digital.library.yorku.ca/api/reconcile` | York-specific records: the YUDL taxonomy vocabularies (Person, Subject, Corporate Body, City, Genre, Language, ...) | YUDL **Term IDs (TIDs)** and labels | YUDL authority pages on `digital.library.yorku.ca` |
| **LoC** | [LoC Reconciliation Service](lc.md) | `https://reconcile.library.yorku.ca/loc/` | Standard library headings: Library of Congress (LCNAF names, LCSH subjects) | **Labels** and stable **URIs** (`id.loc.gov`) | `id.loc.gov` authority records |
| **GeoNames** | [GeoNames Reconciliation Service](geonames.md) | `https://reconcile.library.yorku.ca/geonames/` | Geographic entities, especially when you need coordinates | **Names**, **URIs**, and **coordinates** | `geonames.org` entries |

## Choosing a service

- **Use YUDL** when your data needs to align with York's own taxonomy authorities (for example, content destined for the YUDL digital library with expected TIDs).
- **Use LoC** when you want well-established library authority headings, or if you need to search LCNAF (names) and LCSH (subjects) together via **/LoC**.
- **Use GeoNames** when you are working with place names and need geographic coordinates, or want the broadest search capabilities via **/geonames/all**.

## Common workflow

Regardless of service, reconciliation in OpenRefine follows the same steps:

1. Open the reconciliation dialog from your column.
2. Add the service using its URL.
3. Choose a reconciliation type / vocabulary.
4. Start reconciling and review the candidates.
5. Accept the correct matches (single or double check).
6. Extract the identifier and label into new columns with [GREL expressions](https://openrefine.org/docs/manual/grel) (see each guide for the expressions to use).

## Contents

- [YUDL Reconciliation Service](yudl.md) — reconcile against York's taxonomy authorities and retrieve TIDs.
- [LoC Reconciliation Service](lc.md) — reconcile against Library of Congress authorities and retrieve labels and URIs.
- [GeoNames Reconciliation Service](geonames.md) — reconcile against GeoNames and retrieve names, URIs, and coordinates.
- [Reconciliation Tips & Troubleshooting](tips.md) — common questions and fixes shared across all three services.
