---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Manage incidents
  version: 1.0.0
  description: Acknowledge, resolve, escalate or reassign one or more incidents.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /incidents:
    get:
      summary: List incidents
      description: List existing incidents.
      operationId: list-existing-incidents
      x-api-path-slug: incidents-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      - in: query
        name: sort_by
        description: Used to specify both the field you wish to sort the results on
          (incident_number/created_on/resolved_on/urgency), as well as the direction
          (asc/desc) of the results
      - in: query
        name: statuses[]
        description: Return only incidents with the given statuses
      responses:
        200:
          description: OK
      tags:
      - Incidents
    put:
      summary: Manage incidents
      description: Acknowledge, resolve, escalate or reassign one or more incidents.
      operationId: acknowledge-resolve-escalate-or-reassign-one-or-more-incidents
      x-api-path-slug: incidents-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Incidents
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