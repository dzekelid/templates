---
swagger: "2.0"
x-collection-name: Azure DevTest Labs
x-complete: 1
info:
  title: DevTestLabsClient
  description: the-devtest-labs-client-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/artifactsources/{artifactSourceName}/armtemplates
  : get:
      summary: Arm Templates List
      description: List azure resource manager templates in a given artifact source.
      operationId: ArmTemplates_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameartifactsourcesartifactsourcenamearmtemplates-get
      parameters:
      - in: query
        name: $expand
        description: Specify the $expand query
      - in: query
        name: $filter
        description: The filter to apply to the operation
      - in: query
        name: $orderby
        description: The ordering expression for the results, using OData notation
      - in: query
        name: $top
        description: The maximum number of resources to return from the operation
      - in: path
        name: artifactSourceName
        description: The name of the artifact source
      - in: path
        name: labName
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ARM Templates
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/artifactsources/{artifactSourceName}/armtemplates/{name}
  : get:
      summary: Arm Templates Get
      description: Get azure resource manager template.
      operationId: ArmTemplates_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabslabnameartifactsourcesartifactsourcenamearmtemplatesname-get
      parameters:
      - in: query
        name: $expand
        description: Specify the $expand query
      - in: path
        name: artifactSourceName
        description: The name of the artifact source
      - in: path
        name: labName
        description: The name of the lab
      - in: path
        name: name
        description: The name of the azure Resource Manager template
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ARM Templates
---