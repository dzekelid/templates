swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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
  /v3/templates/dockerfiles:
    get:
      summary: Get Templates Dockerfiles
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3TemplatesDockerfiles
      x-api-path-slug: v3templatesdockerfiles-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Dockerfiles
  /v3/templates/dockerfiles/{name}:
    get:
      summary: Get Templates Dockerfiles Name
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3TemplatesDockerfilesName
      x-api-path-slug: v3templatesdockerfilesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Dockerfiles
      - Name