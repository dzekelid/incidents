{
  "info": {
    "name": "PagerDuty List incidents",
    "_postman_id": "15e53258-480b-4473-855d-d52e9953c872",
    "description": "List existing incidents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "bb36bd10-a7af-4839-8cc2-d6d3fa7a319d",
          "name": "list-existing-incidents",
          "request": {
            "url": "http://example.com/api/incidents?include=%5B%7B%7D%5D&No Name=%7B%7D&sort_by=%7B%7D&statuses=%5B%7B%7D%5D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List existing incidents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13df0ba0-39fc-47bc-8c99-95bfdfd554a1"
            }
          ]
        }
      ]
    }
  ]
}