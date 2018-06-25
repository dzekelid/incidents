---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: Incidents
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops Get current incident information
  x-api-slug: victor-ops
  description: |-
    Get a list of the currently open, acknowledged and recently resolved incidents.
    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-get-openapi.md
- name: Victor Ops Create a new incident
  x-api-slug: victor-ops
  description: |-
    Create a new incident.

    This call replicates the function of our
    manual incident creation process.
    Monitoring tools and custom integrations
    should be configured using our
    REST Endpoint.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidents-post-openapi.md
- name: Victor Ops Acknowledge an incident or list of incidents
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/ack
  tags: Incidents,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsack-patch-openapi.md
- name: Victor Ops Acknowledge all incidents for which a user was paged.
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/ack
  tags: Incidents,ByUser,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-openapi.md
- name: Victor Ops Resolve all incidents for which a user was paged.
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/resolve
  tags: Incidents,ByUser,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-openapi.md
- name: Victor Ops Reroute one or more incidents to one or more new routable destinations.
  x-api-slug: victor-ops
  description: Reroute one or more incidents to one or more users and/or escalation
    policies
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/reroute
  tags: Incidents,Reroute
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsreroute-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsreroute-post-openapi.md
- name: Victor Ops Resolve an incident or list of incidents
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/resolve
  tags: Incidents,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apipublicv1incidentsresolve-patch-openapi.md
- name: Victor Ops Get/search incident history
  x-api-slug: victor-ops
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__

    Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical
    data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v1/incidents
  tags: Api-reporting,V1,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv1incidents-get-openapi.md
- name: Victor Ops Get/search incident history
  x-api-slug: victor-ops
  description: |-
    Retrieve incident history for your company, searching over date ranges and with filtering options.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    Unless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v2/incidents
  tags: Api-reporting,V2,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv2incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/victorops/apireportingv2incidents-get-openapi.md
- name: Victor Ops
  x-api-slug: victor-ops
  description: VictorOps incident managament software gives DevOps observability,
    collaboration, & real-time alerting, to build, deploy, & operate software. Learn
    more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
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
- type: x-crunchbase
  url: https://crunchbase.com/organization/victorops
- type: x-email
  url: support@victorops.com
- type: x-email
  url: info@victorops.com
- type: x-email
  url: press@victorops.com
- type: x-email
  url: sales@victorops.com
- type: x-github
  url: https://github.com/victorops
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: http://victorops.com
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---