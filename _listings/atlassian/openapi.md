swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /template/blueprint:
    get:
      summary: Get blueprint templates
      description: "Returns all templates provided by blueprints. Use this method
        to retrieve \nall global blueprint templates or all blueprint templates in
        a space.\n\nNote, all global blueprints are inherited by each space. Space
        blueprints \ncan be customised without affecting the global blueprints.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to access the Confluence site ('Can use' global permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.getBlueprintTemplates_get
      x-api-path-slug: templateblueprint-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the templateto
          expand
      - in: query
        name: limit
        description: The maximum number of templates to return per page
      - in: query
        name: spaceKey
        description: The key of the space to be queried for templates
      - in: query
        name: start
        description: The starting index of the returned templates
      responses:
        200:
          description: OK
      tags:
      - Blueprint
      - Templates
  /template/page:
    get:
      summary: Get content templates
      description: "Returns all content templates. Use this method to retrieve all
        global\ncontent templates or all content templates in a space.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Admin' permission for the space to view space templates and
        'Confluence \nAdministrator' global permission to view global templates."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.getContentTemplates_get
      x-api-path-slug: templatepage-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the templateto
          expand
      - in: query
        name: limit
        description: The maximum number of templates to return per page
      - in: query
        name: spaceKey
        description: The key of the space to be queried for templates
      - in: query
        name: start
        description: The starting index of the returned templates
      responses:
        200:
          description: OK
      tags:
      - Content
      - Templates