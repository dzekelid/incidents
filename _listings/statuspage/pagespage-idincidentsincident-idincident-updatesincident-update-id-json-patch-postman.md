{
  "info": {
    "name": "StatusPage.io Tune an Incident Update",
    "_postman_id": "e7b205c0-b8ad-4363-9b91-630e2ef9d57d",
    "description": "Tune an Incident Update",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "b6a23c4c-9f89-4261-b68a-272eb7c78c12",
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
              "id": "e6bd06e7-d4e0-46d5-9d3a-66d1471722b5"
            }
          ]
        },
        {
          "id": "de063994-93e8-4d95-b4fe-eb049c3f8a28",
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
              "id": "27190e01-8dd7-41b4-9ad4-24c3743c3b6e"
            }
          ]
        },
        {
          "id": "2e749686-ac6b-4b51-9337-048458b97d6c",
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
              "id": "2ee21694-0886-4bad-9f76-7f06850fcfac"
            }
          ]
        },
        {
          "id": "4760f2bd-009c-4f5b-b8e7-b01fde5ff95e",
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
              "id": "49ef8b71-e9aa-4932-a9db-5db5c9c9799e"
            }
          ]
        },
        {
          "id": "1962ab93-b74e-43d0-b146-658eb914fd33",
          "name": "delete-an-incident",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an incident"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab4bdbe3-39fd-47dc-b78a-16511246db61"
            }
          ]
        },
        {
          "id": "12c97915-3947-4f8a-a97f-2cc31793b3f6",
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
              "id": "b495b9c6-2e13-41af-843a-e6a1b2a25d3a"
            }
          ]
        },
        {
          "id": "134dab10-0fda-4267-8985-157f3d204a2c",
          "name": "tune-an-incident-update",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id]/incident_updates/[incident_update_id].json?incident_update[body]=incident_update%5Bbody%5D&incident_update[display_at]=incident_update%5Bdisplay_at%5D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Tune an Incident Update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d206bdc-fa01-44c7-a927-100e212e9841"
            }
          ]
        }
      ]
    }
  ]
}