---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Templates Gitlab Ci Ymls Name
  version: 1.0.0
  description: This feature was introduced in GitLab 8.9.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/templates/licenses:
    get:
      summary: Get Templates Licenses
      description: This feature was introduced in GitLab 8.7.
      operationId: getV3TemplatesLicenses
      x-api-path-slug: v3templateslicenses-get
      parameters:
      - in: query
        name: popular
        description: If passed, returns only popular licenses
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Licenses
  /v3/templates/licenses/{name}:
    get:
      summary: Get Templates Licenses Name
      description: This feature was introduced in GitLab 8.7.
      operationId: getV3TemplatesLicensesName
      x-api-path-slug: v3templateslicensesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Licenses
      - Name
  /v3/templates/gitignores:
    get:
      summary: Get Templates Gitignores
      description: This feature was introduced in GitLab 8.8.
      operationId: getV3TemplatesGitignores
      x-api-path-slug: v3templatesgitignores-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitignores
  /v3/templates/gitignores/{name}:
    get:
      summary: Get Templates Gitignores Name
      description: This feature was introduced in GitLab 8.8.
      operationId: getV3TemplatesGitignoresName
      x-api-path-slug: v3templatesgitignoresname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitignores
      - Name
  /v3/templates/gitlab_ci_ymls:
    get:
      summary: Get Templates Gitlab Ci Ymls
      description: This feature was introduced in GitLab 8.9.
      operationId: getV3TemplatesGitlabCiYmls
      x-api-path-slug: v3templatesgitlab-ci-ymls-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitlab
      - Ci
      - Ymls
  /v3/templates/gitlab_ci_ymls/{name}:
    get:
      summary: Get Templates Gitlab Ci Ymls Name
      description: This feature was introduced in GitLab 8.9.
      operationId: getV3TemplatesGitlabCiYmlsName
      x-api-path-slug: v3templatesgitlab-ci-ymlsname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitlab
      - Ci
      - Ymls
      - Name
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