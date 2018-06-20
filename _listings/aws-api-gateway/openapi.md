---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 1
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapis/uojnr9hd57/models/output/default_template:
    get:
      summary: Model Generatetemplate
      description: Generates a sample mapping template that can be used to transform
        a payload into the structure of a model.
      operationId: modelGenerate-template
      x-api-path-slug: restapisuojnr9hd57modelsoutputdefault-template-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Model
      - Templates
---