swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAssessmentTemplates:
    get:
      summary: Describe Assessment Templates
      description: |-
        Describes the assessment templates that are specified by the ARNs of the assessment
                 templates.
      operationId: describeAssessmentTemplates
      x-api-path-slug: actiondescribeassessmenttemplates-get
      parameters:
      - in: query
        name: assessmentTemplateArns
        description: 'Type: array of Strings'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Templates
  /?Action=ListAssessmentTemplates:
    get:
      summary: List Assessment Templates
      description: |-
        Lists the assessment templates that correspond to the assessment targets that are
                 specified by the ARNs of the assessment targets.
      operationId: listAssessmentTemplates
      x-api-path-slug: actionlistassessmenttemplates-get
      parameters:
      - in: query
        name: assessmentTargetArns
        description: A list of ARNs that specifies the assessment targets whose assessment
          templates you         want to list
        type: string
      - in: query
        name: filter
        description: You can use this parameter to specify a subset of data to be
          included in the actions         response
        type: string
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items you want in the         response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Templates