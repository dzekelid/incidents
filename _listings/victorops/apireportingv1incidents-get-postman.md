{
  "info": {
    "name": "VictorOps Get/search incident history",
    "_postman_id": "12bad7a6-9b39-4e93-9266-a8d4deec1f1c",
    "description": "__NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__\n\nRetrieve incident history for your company, searching over date ranges and with filtering options.  This is historical\ndata, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.\n\nThis API may be called a maximum of once a minute.\n\nIncident requests are paginated with a offset and limit query string parameters.\n  The query for incidents is run and offset records are skipped, after which limit records will be returned.\n\nThe default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.\n\nOn return, the total number of records available for that query will be returned in the payload as 'total'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "baa49a2e-f8c7-46f2-93a5-5bad80894bc9",
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
              "id": "6db825a3-160a-45f2-91f5-be3c29f25299"
            }
          ]
        },
        {
          "id": "639095d9-0faf-434f-967e-b2f5dab8fef7",
          "name": "api_public.v1.incidents.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new incident.\n\nThis call replicates the function of our\nmanual incident creation process.\nMonitoring tools and custom integrations\nshould be configured using our\nREST Endpoint.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b6b3e08-6f3c-4c14-9cb2-673b916a2566"
            }
          ]
        },
        {
          "id": "317ffbaa-e0d4-44db-80f7-2ac60dc47d23",
          "name": "api_public.v1.incidents.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91b39ff3-3a61-43b9-8e15-df95c7700e99"
            }
          ]
        },
        {
          "id": "697c54b9-f5a9-4837-929c-f19d2c001e56",
          "name": "api_public.v1.incidents.byUser.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da39d1e9-fb14-4e07-810a-ccd0f28d6d9f"
            }
          ]
        },
        {
          "id": "89512bd0-a410-488e-9553-7d3c80f402ac",
          "name": "api_public.v1.incidents.byUser.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4681b1ad-eb49-4fab-b786-a61667c20ae2"
            }
          ]
        },
        {
          "id": "c0bfbe6f-6b3e-495f-bd1f-d98193712987",
          "name": "api_public.v1.incidents.reroute.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/reroute?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reroute one or more incidents to one or more users and/or escalation policies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9c9640-3e0b-4038-a2e6-30114c18977e"
            }
          ]
        },
        {
          "id": "27c8a5b1-1768-4818-8b37-f1a853f23a16",
          "name": "api_public.v1.incidents.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "744e4a61-7c24-4d4c-827d-7f4f5b1ea5f1"
            }
          ]
        },
        {
          "id": "d7d86be9-9d4a-46ee-b32a-1ad658630ba9",
          "name": "api_reporting.v1.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-reporting/v1/incidents?currentPhase=%7B%7D&entityId=%7B%7D&host=%7B%7D&incidentNumber=%7B%7D&No Name=%7B%7D&service=%7B%7D&startedAfter=%7B%7D&startedBefore=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__\n\nRetrieve incident history for your company, searching over date ranges and with filtering options.  This is historical\ndata, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.\n\nThis API may be called a maximum of once a minute.\n\nIncident requests are paginated with a offset and limit query string parameters.\n  The query for incidents is run and offset records are skipped, after which limit records will be returned.\n\nThe default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.\n\nOn return, the total number of records available for that query will be returned in the payload as 'total'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07f819c8-fcd1-4237-bc2f-d1fcef84ac3a"
            }
          ]
        }
      ]
    }
  ]
}