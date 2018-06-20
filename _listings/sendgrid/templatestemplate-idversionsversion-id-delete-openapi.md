---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Templates Template  Versions Version
  description: |-
    **This endpoint allows you to delete one of your transactional template versions.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string | The ID of the template version |
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
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
      description: |-
        **This endpoint allows you to retrieve all transactional templates.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: GET_templates
      x-api-path-slug: templates-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
    post:
      summary: Add Templates
      description: |-
        **This endpoint allows you to create a transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: POST_templates
      x-api-path-slug: templates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
  /templates/{template_id}:
    delete:
      summary: Delete Templates Template
      description: |-
        **This endpoint allows you to delete a transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.delete
      x-api-path-slug: templatestemplate-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
    get:
      summary: Get Templates Template
      description: |-
        **This endpoint allows you to retrieve a single transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.get
      x-api-path-slug: templatestemplate-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
    patch:
      summary: Patch Templates Template
      description: |-
        **This endpoint allows you to edit a transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.patch
      x-api-path-slug: templatestemplate-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
  /templates/{template_id}/versions:
    post:
      summary: Add Templates Template  Versions
      description: |-
        **This endpoint allows you to create a new version of a template.**

        Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

        For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.versions.post
      x-api-path-slug: templatestemplate-idversions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
      - ""
      - Versions
  /templates/{template_id}/versions/{version_id}:
    delete:
      summary: Delete Templates Template  Versions Version
      description: |-
        **This endpoint allows you to delete one of your transactional template versions.**

        Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

        For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

        ## URI Parameters
        | URI Parameter | Type | Description |
        |---|---|---|
        | template_id | string | The ID of the original template |
        | version_id | string | The ID of the template version |
      operationId: templates.template_id.versions.version_id.delete
      x-api-path-slug: templatestemplate-idversionsversion-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
      - ""
      - Versions
      - Version
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