---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Delete Shipping Templates Shipping Template
  description: Deletes the ShippingTemplate with the given id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/templates/entries/{shipping_template_entry_id}:
    get:
      summary: Get Shipping Templates Entries Shipping Template Entry
      description: Retrieves a ShippingTemplateEntry by id.
      operationId: getShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-get
      parameters:
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    put:
      summary: Put Shipping Templates Entries Shipping Template Entry
      description: Updates a ShippingTemplateEntry
      operationId: putShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    delete:
      summary: Delete Shipping Templates Entries Shipping Template Entry
      description: Deletes a ShippingTemplateEntry
      operationId: deleteShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-delete
      parameters:
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
  /shipping/templates/entries:
    post:
      summary: Post Shipping Templates Entries
      description: Creates a new ShippingTemplateEntry
      operationId: postShippingTemplatesEntries
      x-api-path-slug: shippingtemplatesentries-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: destination_region_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: query
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
  /shipping/templates/{shipping_template_id}:
    get:
      summary: Get Shipping Templates Shipping Template
      description: Retrieves a ShippingTemplate by id.
      operationId: getShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-get
      parameters:
      - in: path
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
    delete:
      summary: Delete Shipping Templates Shipping Template
      description: Deletes the ShippingTemplate with the given id.
      operationId: deleteShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-delete
      parameters:
      - in: path
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
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