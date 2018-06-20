{
  "info": {
    "name": "StatusPage.io Unresolved Only",
    "_postman_id": "66d44221-fdef-4408-9164-08f45b1cc2bd",
    "description": "Unresolved Only",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "038cc39d-5522-4359-82e7-9bc0c3ee8dd9",
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
              "id": "c1f13511-a8f5-423c-89eb-010fd2117684"
            }
          ]
        },
        {
          "id": "7b8c7282-6ca6-4425-b65b-804f14f55659",
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
              "id": "ed3c658e-728e-4bb9-bbd4-ed13a35c68f5"
            }
          ]
        }
      ]
    }
  ]
}