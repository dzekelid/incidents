{
  "info": {
    "name": "StatusPage.io Update an incident (only applies to realtime and scheduled incidents)",
    "_postman_id": "0b992a4b-44e2-4dfb-8a05-3e05bcf08099",
    "description": "Update an incident (only applies to realtime and scheduled incidents)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "b78be167-ef1d-479b-bebd-70d06f9d4f24",
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
              "id": "b5ce12e1-aa30-4e41-95bf-b869d75b4dc5"
            }
          ]
        },
        {
          "id": "4b97fd1e-fa0e-484b-bfae-52b06706024b",
          "name": "create-a-realtime-incident",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents.json?incident[backfilled]=incident%5Bbackfilled%5D&incident[backfill_date]=incident%5Bbackfill_date%5D&incident[component_ids]=incident%5Bcomponent_ids%5D&incident[impact_override]=incident%5Bimpact_override%5D&incident[message]=incident%5Bmessage%5D&incident[name]=incident%5Bname%5D&incident[scheduled_auto_completed]=incident%5Bscheduled_auto_completed%5D&incident[scheduled_auto_in_progress]=incident%5Bscheduled_auto_in_progress%5D&incident[scheduled_for]=incident%5Bscheduled_for%5D&incident[scheduled_remind_prior]=incident%5Bscheduled_remind_prior%5D&incident[scheduled_until]=incident%5Bscheduled_until%5D&incident[status]=incident%5Bstatus%5D&incident[wants_twitter_update]=incident%5Bwants_twitter_update%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a realtime incident"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d41bef8-f464-48f4-9299-41a0556e87d7"
            }
          ]
        },
        {
          "id": "53cefb76-b0fb-4af1-a3be-e5de18bcd877",
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
              "id": "f1531087-00e4-4122-a9f2-473355d75065"
            }
          ]
        },
        {
          "id": "cfb3fbbc-2e4b-4d6c-862c-666ab928a9bb",
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
              "id": "1a49f583-a601-46c8-ba66-5dec405466b5"
            }
          ]
        },
        {
          "id": "dcac4220-6bae-4176-866f-98a1a2bf01fd",
          "name": "update-an-incident-only-applies-to-realtime-and-scheduled-incidents",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id].json?at the same time to avoid two separate incident updates being generated.=at%20the%20same%20time%20to%20avoid%20two%20separate%20incident%20updates%20being%20generated.&ENDPOINT=ENDPOINT&incident[component_ids]=incident%5Bcomponent_ids%5D&incident[impact_override]=incident%5Bimpact_override%5D&incident[message]=incident%5Bmessage%5D&incident[name]=incident%5Bname%5D&incident[status]=incident%5Bstatus%5D&incident[wants_twitter_update]=incident%5Bwants_twitter_update%5D&MUTABLE=MUTABLE&PATCH /pages/[page_id]/incidents/[incident_id].json=PATCH%20%2Fpages%2F%5Bpage_id%5D%2Fincidents%2F%5Bincident_id%5D.json",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Update an incident (only applies to realtime and scheduled incidents)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "860f30dd-2e3c-47a4-9bb2-dc5b666c985d"
            }
          ]
        }
      ]
    }
  ]
}