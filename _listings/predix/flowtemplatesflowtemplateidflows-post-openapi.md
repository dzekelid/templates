---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Post Flow Templates Flowtemplateid Flows
  description: Post flow templates flowtemplateid flows.
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
    post:
      summary: Post Flow Templates
      description: Post flow templates.
      operationId: saveFlowTemplateUsingPOST
      x-api-path-slug: flowtemplates-post
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
  /flow-templates/tags:
    get:
      summary: Get Flow Templates Tags
      description: Get flow templates tags.
      operationId: getAllFlowTemplateTagsUsingGET
      x-api-path-slug: flowtemplatestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Tags
  /flow-templates/{flowTemplateId}:
    get:
      summary: Get Flow Templates Flowtemplateid
      description: Get flow templates flowtemplateid.
      operationId: getFlowTemplateUsingGET
      x-api-path-slug: flowtemplatesflowtemplateid-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    post:
      summary: Post Flow Templates Flowtemplateid
      description: Post flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateid-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    put:
      summary: Put Flow Templates Flowtemplateid
      description: Put flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPUT
      x-api-path-slug: flowtemplatesflowtemplateid-put
      parameters:
      - in: body
        name: flowTemplate
        description: flowTemplate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    delete:
      summary: Delete Flow Templates Flowtemplateid
      description: Delete flow templates flowtemplateid.
      operationId: deleteFlowTemplateUsingDELETE
      x-api-path-slug: flowtemplatesflowtemplateid-delete
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
  /flow-templates/{flowTemplateId}/download:
    get:
      summary: Get Flow Templates Flowtemplateid Download
      description: Get flow templates flowtemplateid download.
      operationId: getFlowTemplateFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateiddownload-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Download
  /flow-templates/{flowTemplateId}/flows:
    get:
      summary: Get Flow Templates Flowtemplateid Flows
      description: Get flow templates flowtemplateid flows.
      operationId: getFlowsUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
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
      - Flowtemplateid
      - Flows
    post:
      summary: Post Flow Templates Flowtemplateid Flows
      description: Post flow templates flowtemplateid flows.
      operationId: saveFlowUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: query
        name: launch
        description: launch
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
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