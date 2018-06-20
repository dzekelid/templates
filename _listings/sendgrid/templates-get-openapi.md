---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Templates
  description: |-
    **This endpoint allows you to retrieve all transactional templates.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
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