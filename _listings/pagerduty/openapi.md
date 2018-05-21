---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
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
  /incidents/{id}:
    get:
      summary: Get an incident
      description: Show detailed information about an incident. Accepts either an
        incident id, or an incident number.
      operationId: show-detailed-information-about-an-incident-accepts-either-an-incident-id-or-an-incident-number
      x-api-path-slug: incidentsid-get
      parameters:
      - in: path
        name: id
        description: Either the id or number of the incident to retrieve
      responses:
        200:
          description: OK
      tags:
      - Incidents
    put:
      summary: Update an incident
      description: Acknowledge, resolve, escalate or reassign an incident.
      operationId: acknowledge-resolve-escalate-or-reassign-an-incident
      x-api-path-slug: incidentsid-put
      parameters:
      - in: path
        name: id
        description: The id of the incident to update
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
  /incidents/{id}/log_entries:
    get:
      summary: List log entries for the incident
      description: List log entries for the specified incident.
      operationId: list-log-entries-for-the-specified-incident
      x-api-path-slug: incidentsidlog-entries-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Incidents Log Entries
---