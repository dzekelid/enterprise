swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListEntitiesForPolicy:
    get:
      summary: List Entities For Policy
      description: |-
        Lists all IAM users, groups, and roles that the specified managed policy is attached
              to.
      operationId: listEntitiesForPolicy
      x-api-path-slug: actionlistentitiesforpolicy-get
      parameters:
      - in: query
        name: EntityFilter
        description: The entity type to use for filtering the results
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy for which you
          want the      versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Entities For Policies