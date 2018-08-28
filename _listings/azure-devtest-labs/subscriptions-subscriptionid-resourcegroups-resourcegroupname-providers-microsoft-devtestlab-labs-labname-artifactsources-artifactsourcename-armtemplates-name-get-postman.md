{
  "info": {
    "name": "Azure DevTest Labs API Arm Templates Get",
    "_postman_id": "66d79c43-b0a9-4ac5-babe-68ca88ed634d",
    "description": "Get azure resource manager template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "arm templates",
      "item": [
        {
          "id": "2ab4b085-cb0b-4db3-a379-4dba253604f7",
          "name": "ArmTemplates_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/artifactsources/:artifactSourceName/armtemplates/:name"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "artifactSourceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get azure resource manager template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8f5356b-1ea2-48ae-97ac-ea1dada813ce"
            }
          ]
        }
      ]
    }
  ]
}