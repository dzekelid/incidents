---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: VictorOps Get/search incident history
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__

    Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical
    data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
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
  /api-public/v1/incidents/byUser/ack:
    patch:
      summary: Acknowledge all incidents for which a user was paged.
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.byUser.ack.patch
      x-api-path-slug: apipublicv1incidentsbyuserack-patch
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
      - ByUser
      - Ack
  /api-public/v1/incidents/byUser/resolve:
    patch:
      summary: Resolve all incidents for which a user was paged.
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.byUser.resolve.patch
      x-api-path-slug: apipublicv1incidentsbyuserresolve-patch
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
      - ByUser
      - Resolve
  /api-public/v1/incidents/reroute:
    post:
      summary: Reroute one or more incidents to one or more new routable destinations.
      description: Reroute one or more incidents to one or more users and/or escalation
        policies
      operationId: api_public.v1.incidents.reroute.post
      x-api-path-slug: apipublicv1incidentsreroute-post
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
      - Reroute
  /api-public/v1/incidents/resolve:
    patch:
      summary: Resolve an incident or list of incidents
      description: |-
        The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.incidents.resolve.patch
      x-api-path-slug: apipublicv1incidentsresolve-patch
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
      - Resolve
  /api-reporting/v1/incidents:
    get:
      summary: Get/search incident history
      description: |-
        __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__

        Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical
        data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.

        This API may be called a maximum of once a minute.

        Incident requests are paginated with a offset and limit query string parameters.
          The query for incidents is run and offset records are skipped, after which limit records will be returned.

        The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

        On return, the total number of records available for that query will be returned in the payload as 'total'.
      operationId: api_reporting.v1.incidents.get
      x-api-path-slug: apireportingv1incidents-get
      parameters:
      - in: query
        name: currentPhase
        description: The current phase of the incident resolved, triggered or acknowledged
      - in: query
        name: entityId
        description: The entity ID involved  This is the unique identifier for the
          entity causing the incident
      - in: query
        name: host
        description: The host involved in the incident Multiple values can be separated
          with commas
      - in: query
        name: incidentNumber
        description: 'The incident number as shown in VictorOps Multiple values and
          ranges are allowed: 4,5,20:50'
      - in: query
        name: No Name
      - in: query
        name: service
        description: The service involved in the incident (if any) Multiple values
          can be separated with commas
      - in: query
        name: startedAfter
        description: Return incidents started after this timestamp Specify the timestamp
          in ISO8601 format
      - in: query
        name: startedBefore
        description: Find incidents started before this timestamp  Specify the timestamp
          in ISO8601 format
      responses:
        200:
          description: OK
      tags:
      - Continuous Deployment
      - Continuous Integration
      - Orchestration
      - Api-reporting
      - V1
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