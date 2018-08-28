---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Post Templates
  description: Post templates.
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /templates:
    get:
      summary: Get Templates
      description: Get templates.
      operationId: getTemplates
      x-api-path-slug: templates-get
      parameters:
      - in: query
        name: Count
        description: The number of Templates to return
      - in: query
        name: Offset
        description: The number of Templates to skip before returning results
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Templates
    post:
      summary: Post Templates
      description: Post templates.
      operationId: postTemplates
      x-api-path-slug: templates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
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