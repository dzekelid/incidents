---
name: Washington Metropolitan Area Transit Authority
x-slug: washington-metropolitan-area-transit-authority
description: The collection of data offered here allows developers to create new and
  innovative applications for the web or mobile devices. We encourage you to integrate
  Metro data into your applications and mashups to help get people the information
  they want about getting around. Use of our APIs and other data is free of charge,
  you have two options, for new developers who want to try out the WMATA API but are
  not ready for production, and you can use our demonstration key, without having
  to register.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
x-kinRank: "8"
x-alexaRank: ""
tags: Incidents
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/apis.md
specificationVersion: "0.14"
apis:
- name: WMATA Incidents JSON - Bus Incidents
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns a set of reported bus incidents/delays
    for a given Route. Omit the\r\nRoute to return all reported items.\r\n\r\nNote
    that the Route parameter accepts only base route names and no\r\nvariations, i.e.:
    use 10A instead of 10Av1 and 10Av2.\r\n\r\nBus incidents/delays are refreshed
    once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nBusIncidents\r\n\r\n\r\nArray
    containing bus incident information (BusIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nBusIncident\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate
    and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:ss
    format (e.g.: 2014-10-28T08:13:03).\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text
    description of the delay or incident.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique
    identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description
    of the incident type. Usually\r\nDelay or Alert but is subject to change at any
    time.\r\n\r\n\r\n\r\nRoutesAffected\r\n\r\nArray containing routes affected. Routes
    listed are usually\r\nidentical to base route names (i.e.: not 10Av1 or 10Av2,
    but 10A),\r\nbut may differ from what our bus methods return."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//json/BusIncidents
  tags: Transit,Buses,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonbusincidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonbusincidents-get-openapi.md
- name: WMATA Incidents JSON - Elevator/Escalator Outages
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns a list of reported elevator and escalator
    outages at a\r\ngiven station. Omit the StationCode parameter to return all reported\r\noutages.\r\n\r\nNote
    that for stations with multiple platforms and therefore StationCodes\r\n(e.g.:
    Metro Center, L'Enfant Plaza, etc.), a distinct call is required for\r\neach StationCode.\r\n\r\nElevator
    and escalator outages are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse
    Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncidents\r\n\r\n\r\nArray
    containing elevator/escalator outage information\r\n(ElevatorIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncident
    Elements\r\n\r\n\r\n\r\n\r\n\r\nDateOutOfServ\r\n\r\nDate and time (Eastern Standard
    Time) unit was reported out of\r\nservice. Will be in YYYY-MM-DDTHH:mm:ss format
    (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time
    (Eastern Standard Time) outage details was last\r\nupdated. Will be in YYYY-MM-DDTHH:mm:ss
    format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDisplayOrder\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nLocationDescription\r\n\r\nFree-text
    description of the unit location within a station\r\n(e.g.: Escalator between
    mezzanine and\r\nplatform).\r\n\r\n\r\n\r\nStationCode\r\n\r\nUnit's station code.
    Use this value in other rail-related APIs\r\nto retrieve data about a station.\r\n\r\n\r\n\r\nStationName\r\n\r\nFull
    station name, may include entrance information (e.g.:\r\nMetro Center, G and 11th
    St\r\nEntrance).\r\n\r\n\r\n\r\nSymptomCode\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nSymptomDescription\r\n\r\nDescription
    for why the unit is out of service or otherwise in\r\nreduced operation.\r\n\r\n\r\n\r\nTimeOutOfService\r\n\r\nDeprecated.
    Use the time\r\nportion of the DateOutOfServ element.\r\n\r\n\r\n\r\nUnitName\r\n\r\nUnique
    identifier for unit, by type (a single elevator and\r\nescalator may have the
    same UnitName, but no two elevators or two\r\nescalators will have the same UnitName).\r\n\r\n\r\n\r\nUnitStatus\r\n\r\nDeprecated.
    If listed here,\r\nthe unit is inoperational or otherwise impaired.\r\n\r\n\r\n\r\nUnitType\r\n\r\nType
    of unit. Will be ELEVATOR\r\nor ESCALATOR."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//json/ElevatorIncidents
  tags: Transit,Elevator,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonelevatorincidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonelevatorincidents-get-openapi.md
- name: WMATA Incidents JSON - Rail Incidents
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns reported rail incidents (significant disruptions
    and delays to\r\nnormal service). The data is identical to WMATA's Metrorail Service
    Status\r\nfeed.\r\n\r\nRail incidents are refreshed once every 20 to 30 seconds
    approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nIncidents\r\n\r\n\r\nArray
    containing rail disruption information (Incident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nIncident
    Elements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard
    Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:SS format (e.g.: 2010-07-29T14:21:28).\r\n\r\n\r\n\r\nDelaySeverity\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text
    description of the incident.\r\n\r\n\r\n\r\nEmergencyText\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nEndLocationFullName\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique
    identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description
    of the incident type. Usually Delay or\r\nAlert but is subject to change at any
    time.\r\n\r\n\r\n\r\nLinesAffected\r\n\r\nSemi-colon and space separated list
    of line codes (e.g.:\r\nRD; or BL;\r\nOR; or BL; OR; RD;). We do\r\nplan to update
    this to return something more reasonable like an\r\narray, but until then, use
    code similar to the following:\r\n\r\n\"RD; GR; BL;\".split(/;[\\s]?/).filter(function(fn)
    { return fn\r\n!== ''; })\r\n\r\n\r\n\r\nPassengerDelay\r\n\r\nDeprecated.\r\n\r\n\r\n\r\n\r\nStartLocationFullName\r\n\r\nDeprecated."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//json/Incidents
  tags: Transit,Buses,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonincidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/jsonincidents-get-openapi.md
- name: WMATA Incidents XML - Bus Incidents
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns a set of reported bus incidents/delays
    for a given Route. Omit the\r\nRoute to return all reported items.\r\n\r\nNote
    that the Route parameter accepts only base route names and no\r\nvariations, i.e.:
    use 10A instead of 10Av1 and 10Av2.\r\n\r\nBus incidents/delays are refreshed
    once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nBusIncidents\r\n\r\n\r\nArray
    containing bus incident information (BusIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nBusIncident\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate
    and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:ss
    format (e.g.: 2014-10-28T08:13:03).\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text
    description of the delay or incident.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique
    identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description
    of the incident type. Usually\r\nDelay or Alert but is subject to change at any
    time.\r\n\r\n\r\n\r\nRoutesAffected\r\n\r\nArray containing routes affected. Routes
    listed are usually\r\nidentical to base route names (i.e.: not 10Av1 or 10Av2,
    but 10A),\r\nbut may differ from what our bus methods return."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//BusIncidents
  tags: Transit,Buses,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/busincidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/busincidents-get-openapi.md
- name: WMATA Incidents XML - Elevator/Escalator Outages
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns a list of reported elevator and escalator
    outages at a\r\ngiven station. Omit the StationCode parameter to return all reported\r\noutages.\r\n\r\nNote
    that for stations with multiple platforms and therefore StationCodes\r\n(e.g.:
    Metro Center, L'Enfant Plaza, etc.), a distinct call is required for\r\neach StationCode.\r\n\r\nElevator
    and escalator outages are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse
    Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncidents\r\n\r\n\r\nArray
    containing elevator/escalator outage information\r\n(ElevatorIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncident
    Elements\r\n\r\n\r\n\r\n\r\n\r\nDateOutOfServ\r\n\r\nDate and time (Eastern Standard
    Time) unit was reported out of\r\nservice. Will be in YYYY-MM-DDTHH:mm:ss format
    (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time
    (Eastern Standard Time) outage details was last\r\nupdated. Will be in YYYY-MM-DDTHH:mm:ss
    format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDisplayOrder\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nLocationDescription\r\n\r\nFree-text
    description of the unit location within a station\r\n(e.g.: Escalator between
    mezzanine and\r\nplatform).\r\n\r\n\r\n\r\nStationCode\r\n\r\nUnit's station code.
    Use this value in other rail-related APIs\r\nto retrieve data about a station.\r\n\r\n\r\n\r\nStationName\r\n\r\nFull
    station name, may include entrance information (e.g.:\r\nMetro Center, G and 11th
    St\r\nEntrance).\r\n\r\n\r\n\r\nSymptomCode\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nSymptomDescription\r\n\r\nDescription
    for why the unit is out of service or otherwise in\r\nreduced operation.\r\n\r\n\r\n\r\nTimeOutOfService\r\n\r\nDeprecated.
    Use the time\r\nportion of the DateOutOfServ element.\r\n\r\n\r\n\r\nUnitName\r\n\r\nUnique
    identifier for unit, by type (a single elevator and\r\nescalator may have the
    same UnitName, but no two elevators or two\r\nescalators will have the same UnitName).\r\n\r\n\r\n\r\nUnitStatus\r\n\r\nDeprecated.
    If listed here,\r\nthe unit is inoperational or otherwise impaired.\r\n\r\n\r\n\r\nUnitType\r\n\r\nType
    of unit. Will be ELEVATOR\r\nor ESCALATOR."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//ElevatorIncidents
  tags: Transit,Elevator,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/elevatorincidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/elevatorincidents-get-openapi.md
- name: WMATA Incidents XML - Rail Incidents
  x-api-slug: wmata-incidents
  description: "Description\r\n\r\nReturns reported rail incidents (significant disruptions
    and delays to\r\nnormal service). The data is identical to WMATA's Metrorail Service
    Status\r\nfeed.\r\n\r\nRail incidents are refreshed once every 20 to 30 seconds
    approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nIncidents\r\n\r\n\r\nArray
    containing rail disruption information (Incident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nIncident
    Elements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard
    Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:SS format (e.g.: 2010-07-29T14:21:28).\r\n\r\n\r\n\r\nDelaySeverity\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text
    description of the incident.\r\n\r\n\r\n\r\nEmergencyText\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nEndLocationFullName\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique
    identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description
    of the incident type. Usually Delay or\r\nAlert but is subject to change at any
    time.\r\n\r\n\r\n\r\nLinesAffected\r\n\r\nSemi-colon and space separated list
    of line codes (e.g.:\r\nRD; or BL;\r\nOR; or BL; OR; RD;). We do\r\nplan to update
    this to return something more reasonable like an\r\narray, but until then, use
    code similar to the following:\r\n\r\n\"RD; GR; BL;\".split(/;[\\s]?/).filter(function(fn)
    { return fn\r\n!== ''; })\r\n\r\n\r\n\r\nPassengerDelay\r\n\r\nDeprecated.\r\n\r\n\r\n\r\n\r\nStartLocationFullName\r\n\r\nDeprecated."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc//Incidents
  tags: Transit,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/incidents-get-openapi.md
- name: WMATA Incidents
  x-api-slug: wmata-incidents
  description: The collection of data offered here allows developers to create new
    and innovative applications for the web or mobile devices. We encourage you to
    integrate Metro data into your applications and mashups to help get people the
    information they want about getting around. Use of our APIs and other data is
    free of charge, you have two options, for new developers who want to try out the
    WMATA API but are not ready for production, and you can use our demonstration
    key, without having to register.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/metro-developers.png
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Incidents.svc
  tags: Incidents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/incidents/master/_listings/washington-metropolitan-area-transit-authority/openapi.md
x-common:
- type: x-base
  url: http://api.wmata.com/
- type: x-developer
  url: http://developer.wmata.com/
- type: x-signup
  url: https://developer.wmata.com/signup/
- type: x-website
  url: http://wmata.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---