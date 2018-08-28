---
swagger: "2.0"
x-collection-name: StatusPage
x-complete: 0
info:
  title: StatusPage.io Get a list of all incidents
  version: 1.0.0
  description: Get a list of all incidents
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages/[page_id]/incidents.json:
    get:
      summary: Get a list of all incidents
      description: Get a list of all incidents
      operationId: get-a-list-of-all-incidents
      x-api-path-slug: pagespage-idincidents-json-get
      responses:
        200:
          description: OK
      tags:
      - Incidents
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---