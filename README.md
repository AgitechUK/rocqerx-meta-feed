# ROCQERX — Meta catalog feed

Machine-generated product feed for the Meta (Facebook/Instagram) catalog
`770199862581643`, fetched on a schedule by Meta Commerce Manager.

- `meta-catalog.csv` — regenerated daily from Shopify by
  `scripts/meta_feed.py` in the ads-automation project.
- `id` is the Shopify variant id, `item_group_id` the Shopify product id, so the
  rows line up with the identifiers the catalog and its product sets already use.

This exists because the Shopify partner integration stopped updating the catalog
at the rocqerxmen.co.uk → rocqerx.com migration and could not be revived; while
that integration owned the fields, Meta refused API corrections to price and URL.

Contains only product data already public on the storefront: titles,
descriptions, prices, stock state, product URLs and image URLs. No credentials,
no customer data, no business metrics.

The history is intentionally a single commit — the file is a regenerated
artifact, amended and force-pushed on each run to keep the repository small.
