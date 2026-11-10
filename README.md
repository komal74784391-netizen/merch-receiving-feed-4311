# Vantage Ridge Receiving Feed — Batch RCV-4311-B7

This repository publishes the regional receiving feed for the current replenishment batch.

Pagination contract:
- each page file carries `pageSize`, `totalResults` and `nextPageToken`;
- `nextPageToken` names the next page file in the `feed/` directory, and `null` marks the last page;
- `feed/catalog-summary.json` reconciles the record counts expected for the batch.

Files:
- `feed/page-1.json` — first feed page
- `feed/page-2.json` — continuation page
- `feed/hub-regions.json` — receiving hub to sales-region mapping
- `feed/catalog-summary.json` — batch reconciliation summary
