---
name: StatusPage.io
x-slug: statuspageio
description: StatusPage.io launched in 2013 to give companies a better way to be more
  transparent with their customers. We recognize managing a status page outside of
  ones own infrastructure can be a hassle, and hope to increase the transparency of
  the web by making it easier to do so.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
x-kinRank: "8"
x-alexaRank: ""
tags: Incidents
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/apis.md
specificationVersion: "0.14"
apis:
- name: StatusPage.io Get a list of all incidents
  x-api-slug: statuspageio
  description: Get a list of all incidents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents.json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsjson-get-openapi.md
- name: StatusPage.io Unresolved Only
  x-api-slug: statuspageio
  description: Unresolved Only
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents/unresolved.json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsunresolvedjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsunresolvedjson-get-openapi.md
- name: StatusPage.io Scheduled Only
  x-api-slug: statuspageio
  description: Scheduled Only
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents/scheduled.json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsscheduledjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsscheduledjson-get-openapi.md
- name: StatusPage.io Create a realtime incident
  x-api-slug: statuspageio
  description: Create a realtime incident
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents.json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsjson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsjson-post-openapi.md
- name: StatusPage.io Update an incident (only applies to realtime and scheduled incidents)
  x-api-slug: statuspageio
  description: Update an incident (only applies to realtime and scheduled incidents)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents/[incident_id].json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idjson-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idjson-patch-openapi.md
- name: StatusPage.io Delete an incident
  x-api-slug: statuspageio
  description: Delete an incident
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents/[incident_id].json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idjson-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idjson-delete-openapi.md
- name: StatusPage.io Tune an Incident Update
  x-api-slug: statuspageio
  description: Tune an Incident Update
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/incidents/[incident_id]/incident_updates/[incident_update_id].json
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idincident-updatesincident-update-idjson-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/pagespage-idincidentsincident-idincident-updatesincident-update-idjson-patch-openapi.md
- name: StatusPage.io
  x-api-slug: statuspageio
  description: StatusPage.io launched in 2013 to give companies a better way to be
    more transparent with their customers. We recognize managing a status page outside
    of ones own infrastructure can be a hassle, and hope to increase the transparency
    of the web by making it easier to do so.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/status-page-io-icon.png
  humanURL: https://www.statuspage.io/
  baseURL: https:///
  tags: Incidents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/statuspageio/openapi.md
x-common:
- type: x-authentication
  url: http://doers.statuspage.io/api/authentication/
- type: x-blog
  url: http://blog.statuspage.io
- type: x-blog-rss
  url: http://blog.statuspage.io/posts.rss
- type: x-developer
  url: http://doers.statuspage.io/
- type: x-github
  url: https://github.com/statuspage
- type: x-pricing
  url: https://www.statuspage.io/pricing
- type: x-privacy
  url: https://www.statuspage.io/privacy-policy
- type: x-security
  url: https://www.statuspage.io/security
- type: x-status
  url: http://metastatuspage.com/
- type: x-terms-of-service
  url: https://www.statuspage.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/statuspageio
- type: x-website
  url: https://www.statuspage.io/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---