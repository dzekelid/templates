---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Flow Templates
  description: Get flow templates.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flow-templates:
    get:
      summary: Get Flow Templates
      description: Get flow templates.
      operationId: getFlowTemplatesUsingGET
      x-api-path-slug: flowtemplates-get
      parameters:
      - in: query
        name: displayShellTemplates
        description: displayShellTemplates
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
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