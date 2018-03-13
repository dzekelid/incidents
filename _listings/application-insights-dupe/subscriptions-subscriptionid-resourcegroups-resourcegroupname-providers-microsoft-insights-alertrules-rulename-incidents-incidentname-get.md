---
swagger: "2.0"
info:
  title: InsightsManagementClient
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/microsoft.insights/alertrules/{ruleName}/incidents/{incidentName}
  : get:
      summary: Get Incident
      description: Gets an incident associated to an alert rule
      operationId: AlertRuleIncidents_Get
      parameters:
      - in: path
        name: incidentName
        description: The name of the incident to retrieve
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - incidents
definitions:
  RuleCondition:
    properties:
      odata.type:
        description: This is a default description.
        type: get
  RuleDataSource:
    properties:
      odata.type:
        description: This is a default description.
        type: get
  RuleMetricDataSource:
    properties:
      resourceUri:
        description: This is a default description.
        type: get
      metricName:
        description: This is a default description.
        type: get
  RuleManagementEventClaimsDataSource:
    properties:
      emailAddress:
        description: This is a default description.
        type: get
  RuleManagementEventDataSource:
    properties:
      eventName:
        description: This is a default description.
        type: get
      eventSource:
        description: This is a default description.
        type: get
      level:
        description: This is a default description.
        type: get
      operationName:
        description: This is a default description.
        type: get
      resourceGroupName:
        description: This is a default description.
        type: get
      resourceProviderName:
        description: This is a default description.
        type: get
      resourceUri:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      subStatus:
        description: This is a default description.
        type: get
  ThresholdRuleCondition:
    properties:
      threshold:
        description: This is a default description.
        type: get
      windowSize:
        description: This is a default description.
        type: get
  LocationThresholdRuleCondition:
    properties:
      windowSize:
        description: This is a default description.
        type: get
      failedLocationCount:
        description: This is a default description.
        type: get
  ManagementEventAggregationCondition:
    properties:
      threshold:
        description: This is a default description.
        type: get
      windowSize:
        description: This is a default description.
        type: get
  ManagementEventRuleCondition:
    properties: []
  RuleAction:
    properties:
      odata.type:
        description: This is a default description.
        type: get
  RuleEmailAction:
    properties:
      sendToServiceOwners:
        description: This is a default description.
        type: get
      customEmails:
        description: This is a default description.
        type: get
  RuleWebhookAction:
    properties:
      serviceUri:
        description: This is a default description.
        type: get
      properties:
        description: This is a default description.
        type: get
  AlertRule:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      isEnabled:
        description: This is a default description.
        type: get
      actions:
        description: This is a default description.
        type: get
      lastUpdatedTime:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  AlertRuleResource:
    properties: []
  AlertRuleResourceCollection:
    properties:
      value:
        description: This is a default description.
        type: get
  Incident:
    properties:
      name:
        description: This is a default description.
        type: get
      ruleName:
        description: This is a default description.
        type: get
      isActive:
        description: This is a default description.
        type: get
      activatedTime:
        description: This is a default description.
        type: get
      resolvedTime:
        description: This is a default description.
        type: get
  IncidentListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  RetentionPolicy:
    properties:
      enabled:
        description: This is a default description.
        type: get
      days:
        description: This is a default description.
        type: get
  LogProfileProperties:
    properties:
      storageAccountId:
        description: This is a default description.
        type: get
      serviceBusRuleId:
        description: This is a default description.
        type: get
      locations:
        description: This is a default description.
        type: get
      categories:
        description: This is a default description.
        type: get
  LogProfileResource:
    properties: []
  LogProfileCollection:
    properties:
      value:
        description: This is a default description.
        type: get
x-collection-name: Application Insights DUPE
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