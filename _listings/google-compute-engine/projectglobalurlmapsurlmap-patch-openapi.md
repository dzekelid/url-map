---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Update URL Map
  description: Updates the specified UrlMap resource with the data included in the
    request. This method supports patch semantics.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/urlMaps:
    get:
      summary: Get URL Maps
      description: Retrieves the list of UrlMap resources available to the specified
        project.
      operationId: compute.urlMaps.list
      x-api-path-slug: projectglobalurlmaps-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - URL Map
    post:
      summary: Create URL Map
      description: Creates a UrlMap resource in the specified project using the data
        included in the request.
      operationId: compute.urlMaps.insert
      x-api-path-slug: projectglobalurlmaps-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - URL Map
  /{project}/global/urlMaps/{urlMap}:
    delete:
      summary: Delete URL Map
      description: Deletes the specified UrlMap resource.
      operationId: compute.urlMaps.delete
      x-api-path-slug: projectglobalurlmapsurlmap-delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: urlMap
        description: Name of the UrlMap resource to delete
      responses:
        200:
          description: OK
      tags:
      - URL Map
    get:
      summary: Get URL Map
      description: Returns the specified UrlMap resource. Get a list of available
        URL maps by making a list() request.
      operationId: compute.urlMaps.get
      x-api-path-slug: projectglobalurlmapsurlmap-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: urlMap
        description: Name of the UrlMap resource to return
      responses:
        200:
          description: OK
      tags:
      - URL Map
    patch:
      summary: Update URL Map
      description: Updates the specified UrlMap resource with the data included in
        the request. This method supports patch semantics.
      operationId: compute.urlMaps.patch
      x-api-path-slug: projectglobalurlmapsurlmap-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: urlMap
        description: Name of the UrlMap resource to update
      responses:
        200:
          description: OK
      tags:
      - URL Map
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