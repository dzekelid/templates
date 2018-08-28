---
swagger: "2.0"
x-collection-name: API Science
x-complete: 0
info:
  title: API Science Get a Template
  version: 1.0.0
  description: Get a Template
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitors/{id}/templates:
    get:
      summary: Show a Monitors Templates
      description: Show a Monitors Templates
      operationId: showMonitorsTemplates
      x-api-path-slug: monitorsidtemplates-get
      parameters:
      - in: path
        name: id
        description: The id for the monitor
      responses:
        200:
          description: OK
      tags:
      - Templates
  /monitors/{id}/templates/{templates]:
    get:
      summary: Get a Template
      description: Get a Template
      operationId: getTemplate
      x-api-path-slug: monitorsidtemplatestemplates-get
      responses:
        200:
          description: OK
      tags:
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