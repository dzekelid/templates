{
  "info": {
    "name": "Azure DevTest Labs API Arm Templates List",
    "_postman_id": "14cf5be4-9d4a-44e4-8ed0-95c644a96dd0",
    "description": "List azure resource manager templates in a given artifact source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "arm templates",
      "item": [
        {
          "id": "1f997e9e-70b0-4774-b4bc-aa3a9276a9d9",
          "name": "ArmTemplates_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/artifactsources/:artifactSourceName/armtemplates"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$orderby",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
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
            "description": "List azure resource manager templates in a given artifact source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bc91b54-a408-4623-9cfc-5f057a2e3dd6"
            }
          ]
        }
      ]
    }
  ]
}