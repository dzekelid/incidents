---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Alerts Incents. Format
  version: 1.0.0
  description: "This API endpoint returns a list of the Incidents associated with
    your New Relic account.\n\nSee our documentation for a discussion on listing incidents
    \nand output pagination."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_incidents.{format}:
    get:
      summary: Get Alerts Incents. Format
      description: "This API endpoint returns a list of the Incidents associated with
        your New Relic account.\n\nSee our documentation for a discussion on listing
        incidents \nand output pagination."
      operationId: getAlertsIncents.Format
      x-api-path-slug: alerts-incidents-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Incents.
      - Format
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