swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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