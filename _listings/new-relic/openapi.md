swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
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