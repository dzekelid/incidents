{
  "info": {
    "name": "StatusPage.io Create a realtime incident",
    "_postman_id": "c2f302a8-6566-4cd9-866b-cf455e3a5297",
    "description": "Create a realtime incident",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Incidents",
      "item": [
        {
          "id": "90ba2f0b-65f2-41ad-868c-8af205bf7486",
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
              "id": "d90e0b55-6642-453a-ba06-a2e5c0a28eaf"
            }
          ]
        },
        {
          "id": "9f544001-16ab-401f-bf3c-5e411c29d3c8",
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
              "id": "19e1c26f-5104-4f9f-9861-d8106afe24ad"
            }
          ]
        },
        {
          "id": "6df9783b-0148-4537-ad0a-1309b5212a56",
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
              "id": "18cfce0b-c33e-441c-ac53-897912967062"
            }
          ]
        },
        {
          "id": "9bacb9d9-a28c-4c98-8c28-f92971f95d4c",
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
              "id": "1fd9e3e8-fbb2-4ebc-991e-40cdc2425a35"
            }
          ]
        }
      ]
    }
  ]
}