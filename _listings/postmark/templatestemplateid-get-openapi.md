---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Get Templates Template
  description: Get templates template.
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
  /templates/validate:
    post:
      summary: Post Templates Valate
      description: Post templates valate.
      operationId: postTemplatesValate
      x-api-path-slug: templatesvalidate-post
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
      - Validate
  /templates/{templateid}:
    delete:
      summary: Delete Templates Template
      description: Delete templates template.
      operationId: deleteTemplatesTemplate
      x-api-path-slug: templatestemplateid-delete
      parameters:
      - in: path
        name: templateid
        description: The ID for the Template you wish to delete
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Templateid
    get:
      summary: Get Templates Template
      description: Get templates template.
      operationId: getTemplatesTemplate
      x-api-path-slug: templatestemplateid-get
      parameters:
      - in: path
        name: templateid
        description: The ID for the Template you wish to retrieve
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Templateid
    put:
      summary: Put Templates Template
      description: Put templates template.
      operationId: putTemplatesTemplate
      x-api-path-slug: templatestemplateid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: templateid
        description: The ID for the Template you wish to update
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Templateid
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