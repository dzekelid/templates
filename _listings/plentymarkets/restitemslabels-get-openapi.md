---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List item label templates
  description: Lists the ID and name of all item label templates saved in the system.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
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