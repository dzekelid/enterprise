swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateNetworkAclEntry:
    get:
      summary: Create Network Acl Entry
      description: Creates an entry (a rule) in a network ACL with the specified rule
        number.
      operationId: createnetworkaclentry
      x-api-path-slug: actioncreatenetworkaclentry-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkAclId
        description: The ID of the network ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC ACL
  /?Action=DeleteNetworkAclEntry:
    get:
      summary: Delete Network Acl Entry
      description: Deletes the specified ingress or egress entry (rule) from the specified
        network ACL.
      operationId: deletenetworkaclentry
      x-api-path-slug: actiondeletenetworkaclentry-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: NetworkAclId.N
        description: One or more network ACL IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network ACL
  /?Action=ReplaceNetworkAclEntry:
    get:
      summary: Replace Network Acl Entry
      description: Replaces an entry (rule) in a network ACL.
      operationId: replacenetworkaclentry
      x-api-path-slug: actionreplacenetworkaclentry-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: GroupName
        description: A name for the placement group
        type: string
      - in: query
        name: Strategy
        description: The placement strategy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network ACL