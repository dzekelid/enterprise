swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
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
    get:
      summary: Get Enterprise
      description: Retrieves the name and domain of an enterprise.
      operationId: androidenterprise.enterprises.get
      x-api-path-slug: enterprisesenterpriseid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/{enterpriseId}/account:
    put:
      summary: Update Enterprise Account
      description: Sets the account that will be used to authenticate to the API as
        the enterprise.
      operationId: androidenterprise.enterprises.setAccount
      x-api-path-slug: enterprisesenterpriseidaccount-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/{enterpriseId}/unenroll:
    post:
      summary: Unenroll Enterprise
      description: Unenrolls an enterprise from the calling EMM.
      operationId: androidenterprise.enterprises.unenroll
      x-api-path-slug: enterprisesenterpriseidunenroll-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise