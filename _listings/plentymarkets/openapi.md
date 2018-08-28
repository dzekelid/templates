swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
      - Templates
  /rest/listings/option_templates/preview:
    get:
      summary: Get a preview list of option templates
      description: Gets a preview list of all available listing option templates.
      operationId: getRestListingsOptionTemplatesPreview
      x-api-path-slug: restlistingsoption-templatespreview-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - List
      - Of
      - Option
      - Templates