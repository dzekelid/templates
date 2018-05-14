---
swagger: "2.0"
info:
  title: Etsy Put Shipping Templates Shipping Template
  description: Updates a ShippingTemplate
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/templates/{shipping_template_id}:
    put:
      summary: Put Shipping Templates Shipping Template
      description: Updates a ShippingTemplate
      operationId: putShippingTemplatesShippingTemplate
      parameters:
      - in: query
        name: origin_country_id
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - shipping
      - templates
      - shipping
      - template
definitions: []
x-collection-name: Etsy
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