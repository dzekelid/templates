---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Loads an OpenEhr web template.
  description: Loads an openehr web template..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
paths:
  /template/{templateId}:
    delete:
      summary: Deletes an existing OpenEHR template.
      description: Deletes an existing openehr template..
      operationId: deleteTemplate
      x-api-path-slug: templatetemplateid-delete
      parameters:
      - in: path
        name: templateId
        description: The ID of the template to delete
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
    get:
      summary: Loads an OpenEhr web template.
      description: Loads an openehr web template..
      operationId: getTemplate
      x-api-path-slug: templatetemplateid-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the returned web template with
      - in: query
        name: languages
        description: Other languages to include in the returned web template, separated
          by a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
  /template/{templateId}/example:
    get:
      summary: Returns an example of data values for a web template.
      description: Returns an example of data values for a web template..
      operationId: getTemplateExample
      x-api-path-slug: templatetemplateidexample-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the web template with
      - in: query
        name: exampleFilter
        description: The type of example to produce - intended for input (sent to
          the server), output (received back from the server) etc
      - in: query
        name: format
        description: The format of JSON representation of the example composition
          to return
      - in: query
        name: languages
        description: Other languages to include in the web template, separated by
          a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
      - Example
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