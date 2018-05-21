---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: VictorOps Acknowledge an incident or list of incidents
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  version: 1.0.0
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/incidents:
    get:
      summary: Get current incident information
      description: |-
        Get a list of the currently open, acknowledged and recently resolved incidents.
        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.get
      x-api-path-slug: apipublicv1incidents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Incidents
    post:
      summary: Create a new incident
      description: |-
        Create a new incident.

        This call replicates the function of our
        manual incident creation process.
        Monitoring tools and custom integrations
        should be configured using our
        REST Endpoint.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.post
      x-api-path-slug: apipublicv1incidents-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Incidents
  /api-public/v1/incidents/ack:
    patch:
      summary: Acknowledge an incident or list of incidents
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.ack.patch
      x-api-path-slug: apipublicv1incidentsack-patch
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-public
      - V1
      - Incidents
      - Ack
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