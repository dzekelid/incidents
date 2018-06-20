{
  "info": {
    "name": "Victor Ops Get current incident information",
    "_postman_id": "56af32c1-0a1e-4bec-809c-e4322ac2edec",
    "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "ed7c1259-8db0-4493-9e6b-b843fa57ce64",
          "name": "api_public.v1.alerts.uuid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/alerts/:uuid"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the details of an alert that was sent VictorOps by you.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8d69edc-d91c-4ebc-bd4b-956c37c0b6a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "84c6b391-ba53-4c0d-9fb4-24d277afa4d3",
          "name": "api_public.v1.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e178a21e-5054-4050-94ca-644d0fe5df03"
            }
          ]
        }
      ]
    }
  ]
}