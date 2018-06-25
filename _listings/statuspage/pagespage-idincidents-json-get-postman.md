{
  "info": {
    "name": "StatusPage.io Get a list of all incidents",
    "_postman_id": "52fd7b31-2b06-4ccd-80ae-02916c8f35f6",
    "description": "Get a list of all incidents",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "1be0e958-0200-47b5-b879-9acab5934af3",
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
              "id": "f24f11ba-3d4b-4f9e-8c1b-ec0a8cceb046"
            }
          ]
        }
      ]
    }
  ]
}