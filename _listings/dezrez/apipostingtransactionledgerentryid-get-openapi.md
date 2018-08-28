---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get ledger entry details by Id
  version: 1.0.0
  description: Get ledger entry details by id.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/posting/transaction/{ledgerEntryId}:
    get:
      summary: Get ledger entry details by Id
      description: Get ledger entry details by id.
      operationId: Posting_GetTransactionByledgerEntryIdByaccountId
      x-api-path-slug: apipostingtransactionledgerentryid-get
      parameters:
      - in: query
        name: accountId
        description: Account Id to filter ledger lines
      - in: path
        name: ledgerEntryId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Ledger
      - Entry
      - Details
      - By
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---