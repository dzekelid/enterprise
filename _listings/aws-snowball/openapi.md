swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 1
info:
  title: AWS Snowball API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListClusterJobs:
    get:
      summary: List Cluster Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listClusterJobs
      x-api-path-slug: actionlistclusterjobs-get
      parameters:
      - in: query
        name: ClusterId
        description: The 39-character ID for the cluster that you want to list, for
          example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Jobs
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns an array of ClusterListEntry objects of the specified length.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: MaxResults
        description: The number of ClusterListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListJobs:
    get:
      summary: List Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listJobs
      x-api-path-slug: actionlistjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs