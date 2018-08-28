swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/IsPinEntered:
    get:
      summary: Get API Ispinentered
      description: Get api ispinentered.
      operationId: ApiIsPinEnteredGet
      x-api-path-slug: apiispinentered-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ispinentered