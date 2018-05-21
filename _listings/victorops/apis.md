---
name: VictorOps
x-slug: victorops
description: VictorOps is a hub for centralizing the flow of information throughout
  the incident lifecycle. Driven by IT and DevOps system data, VictorOps provides
  a unified platform for real-time alerting, collaboration, and documentation. Using
  VictorOps, teams resolve incidents faster to help minimize the impact of downtime
  and speed innovation.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
x-kinRank: "8"
x-alexaRank: ""
tags: Incidents
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: VictorOps Get current incident information
  x-api-slug: victorops
  description: |-
    Get a list of the currently open, acknowledged and recently resolved incidents.
    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-get-openapi.md
- name: VictorOps Create a new incident
  x-api-slug: victorops
  description: |-
    Create a new incident.

    This call replicates the function of our
    manual incident creation process.
    Monitoring tools and custom integrations
    should be configured using our
    REST Endpoint.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-post-openapi.md
- name: VictorOps Acknowledge an incident or list of incidents
  x-api-slug: victorops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/ack
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsack-patch-openapi.md
- name: VictorOps Acknowledge all incidents for which a user was paged.
  x-api-slug: victorops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/ack
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents,ByUser,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-openapi.md
- name: VictorOps Resolve all incidents for which a user was paged.
  x-api-slug: victorops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/resolve
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents,ByUser,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-openapi.md
- name: VictorOps Reroute one or more incidents to one or more new routable destinations.
  x-api-slug: victorops
  description: Reroute one or more incidents to one or more users and/or escalation
    policies
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/reroute
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents,Reroute
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsreroute-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsreroute-post-openapi.md
- name: VictorOps Resolve an incident or list of incidents
  x-api-slug: victorops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/resolve
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-public,V1,Incidents,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsresolve-patch-openapi.md
- name: VictorOps Get/search incident history
  x-api-slug: victorops
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__

    Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical
    data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v1/incidents
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-reporting,V1,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv1incidents-get-openapi.md
- name: VictorOps Get/search incident history
  x-api-slug: victorops
  description: |-
    Retrieve incident history for your company, searching over date ranges and with filtering options.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    Unless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v2/incidents
  tags: Continuous Deployment,Continuous Integration,Orchestration,Api-reporting,V2,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv2incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv2incidents-get-openapi.md
- name: VictorOps
  x-api-slug: victorops
  description: VictorOps is a hub for centralizing the flow of information throughout
    the incident lifecycle. Driven by IT and DevOps system data, VictorOps provides
    a unified platform for real-time alerting, collaboration, and documentation. Using
    VictorOps, teams resolve incidents faster to help minimize the impact of downtime
    and speed innovation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/victorops.jpg
  humanURL: https://victorops.com
  baseURL: https://api.victorops.com//
  tags: Incidents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/openapi.md
x-common:
- type: x-blog
  url: https://victorops.com/blog/
- type: x-blog-rss
  url: https://victorops.com/feed/
- type: x-github
  url: https://github.com/victorops
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---