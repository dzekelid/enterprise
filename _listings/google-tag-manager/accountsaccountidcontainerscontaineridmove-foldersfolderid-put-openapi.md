---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Move Entity
  description: Moves entities to a GTM Folder.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/containers/{containerId}/folders/{folderId}/entities:
    get:
      summary: Get Entities
      description: List all entities in a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.entities.list
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderidentities-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - Entity
  /accounts/{accountId}/containers/{containerId}/move_folders/{folderId}:
    put:
      summary: Move Entity
      description: Moves entities to a GTM Folder.
      operationId: tagmanager.accounts.containers.move_folders.update
      x-api-path-slug: accountsaccountidcontainerscontaineridmove-foldersfolderid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      - in: query
        name: tagId
        description: The tags to be moved to the folder
      - in: query
        name: triggerId
        description: The triggers to be moved to the folder
      - in: query
        name: variableId
        description: The variables to be moved to the folder
      responses:
        200:
          description: OK
      tags:
      - Entity
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