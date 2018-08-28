---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Traffic API Traffic Incidents via Proximity
  description: |-
    *Request traffic incident information within specified area*

    Traffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.



    * **prox**  `prox`
     \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

    * **criticality**  `multi-enum`
     \- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact

     Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  version: 1.0.0
host: tiles.traffic.cit.api.here.com
basePath: /traffic/6.0/tiles/8/133/86/256
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /6.0/incidents.json:
    get:
      summary: Traffic Incidents via Proximity
      description: |-
        *Request traffic incident information within specified area*

        Traffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.



        * **prox**  `prox`
         \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

        * **criticality**  `multi-enum`
         \- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact

         Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 60IncidentsJsonGet3
      x-api-path-slug: 6-0incidents-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: criticality
      - in: query
        name: prox
      responses:
        200:
          description: OK
      tags:
      - Traffic
      - Incidents
      - Via
      - Proximity
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---