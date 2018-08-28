---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Delete Enterprise
  version: 1.0.0
  description: Deletes the binding between the EMM and enterprise. This is now deprecated.
    Use this method only to unenroll customers that were previously enrolled with
    the insert call, then enroll them again with the enroll call.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises:
    get:
      summary: Get Enterprises
      description: Looks up an enterprise by domain name. This is only supported for
        enterprises created via the Google-initiated creation flow. Lookup of the
        id is not needed for enterprises created via the EMM-initiated flow since
        the EMM learns the enterprise ID in the callback specified in the Enterprises.generateSignupUrl
        call.
      operationId: androidenterprise.enterprises.list
      x-api-path-slug: enterprises-get
      parameters:
      - in: query
        name: domain
        description: The exact primary domain name of the enterprise to look up
      responses:
        200:
          description: OK
      tags:
      - Enterprise
    post:
      summary: Create Enterprise
      description: Establishes the binding between the EMM and an enterprise. This
        is now deprecated; use enroll instead.
      operationId: androidenterprise.enterprises.insert
      x-api-path-slug: enterprises-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: The token provided by the enterprise to register the EMM
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/{enterpriseId}:
    delete:
      summary: Delete Enterprise
      description: Deletes the binding between the EMM and enterprise. This is now
        deprecated. Use this method only to unenroll customers that were previously
        enrolled with the insert call, then enroll them again with the enroll call.
      operationId: androidenterprise.enterprises.delete
      x-api-path-slug: enterprisesenterpriseid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
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