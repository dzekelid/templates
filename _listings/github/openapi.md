swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gitignore/templates:
    get:
      summary: Get Gitignore Templates
      description: |-
        Listing available templates.
        List all templates available to pass as an option when creating a repository.
      operationId: listing-available-templateslist-all-templates-available-to-pass-as-an-option-when-creating-a-reposit
      x-api-path-slug: gitignoretemplates-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - Gitignore
      - Templates
  /gitignore/templates/{language}:
    get:
      summary: Get Gitignore Templates Language
      description: Get a single template.
      operationId: get-a-single-template
      x-api-path-slug: gitignoretemplateslanguage-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: language
      responses:
        200:
          description: OK
      tags:
      - Gitignore
      - Templates
      - Language