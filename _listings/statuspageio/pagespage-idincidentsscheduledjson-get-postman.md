{
  "info": {
    "name": "StatusPage.io Scheduled Only",
    "_postman_id": "940fcdb4-e7c9-4d95-a198-da2db19076da",
    "description": "Scheduled Only",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "d1a6946e-5982-4c39-87b5-e59d172c34a1",
          "name": "get-a-list-of-all-incidents",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all incidents"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79395048-57a3-446b-bdf8-4ed3d0a77dba"
            }
          ]
        },
        {
          "id": "49b15f1f-2105-4cb5-af94-139b7b6189b3",
          "name": "unresolved-only",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/unresolved.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unresolved Only"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a617d37-6713-4777-84dc-d7e4df889fb7"
            }
          ]
        },
        {
          "id": "1cf99109-08a0-4c07-818e-64e9e26f5ec7",
          "name": "scheduled-only",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/scheduled.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Scheduled Only"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf780fe2-7d17-48bb-ba1e-152aae631cb5"
            }
          ]
        }
      ]
    }
  ]
}