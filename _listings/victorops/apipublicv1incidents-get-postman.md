{
  "info": {
    "name": "VictorOps Get current incident information",
    "_postman_id": "551a091c-0862-4147-a4b9-e3d880e3a3f0",
    "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Continuous Deployment",
      "item": [
        {
          "id": "5bdb93aa-993f-4610-8739-67ce80ea04e2",
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
              "id": "8a2dc5b5-7fdf-483f-a6ba-c74728bcf01b"
            }
          ]
        }
      ]
    }
  ]
}