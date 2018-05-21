{
  "info": {
    "name": "VictorOps Get/search incident history",
    "_postman_id": "2ad3991e-e50a-4a70-b3ee-1001d97611b0",
    "description": "Retrieve incident history for your company, searching over date ranges and with filtering options.\n\nThis API may be called a maximum of once a minute.\n\nIncident requests are paginated with a offset and limit query string parameters.\n  The query for incidents is run and offset records are skipped, after which limit records will be returned.\n\nThe default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.\n\nUnless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.\n\nOn return, the total number of records available for that query will be returned in the payload as 'total'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "7b1357bf-b9a0-4c57-bdb9-71ace022da29",
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
              "id": "3870728e-0052-453f-836a-110b365eace8"
            }
          ]
        },
        {
          "id": "c23f986c-e231-42d4-b535-b2cacafb3677",
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
              "id": "d7d8c0e4-dcfe-403c-8c77-39af9f4a96e4"
            }
          ]
        },
        {
          "id": "91bdfcb2-4193-466a-97f7-100cc04dbff0",
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
              "id": "867372ed-03e5-4ccd-bf97-5667573ef0ae"
            }
          ]
        },
        {
          "id": "bec740f2-45ea-4ba6-b005-52c52251dc5b",
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
              "id": "fb4868b1-f207-47e4-9cca-757b3901d9e1"
            }
          ]
        },
        {
          "id": "54774e58-1970-4333-a950-da17ddb05901",
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
              "id": "594ec5a0-d9c8-43c8-95f8-84cc9e59bcb2"
            }
          ]
        },
        {
          "id": "321ffb62-7f50-4a79-92b8-f1fd2b9a359e",
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
              "id": "4c9c4a66-8319-409d-9a4a-592389054592"
            }
          ]
        },
        {
          "id": "fc3ae4de-bfef-449a-81dd-08319b6fe894",
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
              "id": "2b27ba25-88d5-4253-8d9f-4ccfc0e6d110"
            }
          ]
        },
        {
          "id": "69ca7de1-3fea-4915-915b-cce3f582f591",
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
              "id": "d78e7607-71f5-489f-92af-1c751d5a5aac"
            }
          ]
        },
        {
          "id": "2a4cbb05-7c9f-465f-b7ab-04a2a28c97b7",
          "name": "api_reporting.v2.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-reporting/v2/incidents?currentPhase=%7B%7D&entityId=%7B%7D&host=%7B%7D&incidentNumber=%7B%7D&No Name=%7B%7D&routingKey=%7B%7D&service=%7B%7D&startedAfter=%7B%7D&startedBefore=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve incident history for your company, searching over date ranges and with filtering options.\n\nThis API may be called a maximum of once a minute.\n\nIncident requests are paginated with a offset and limit query string parameters.\n  The query for incidents is run and offset records are skipped, after which limit records will be returned.\n\nThe default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.\n\nUnless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.\n\nOn return, the total number of records available for that query will be returned in the payload as 'total'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d5b57b4-d908-45b4-81e4-90a067538c9d"
            }
          ]
        }
      ]
    }
  ]
}