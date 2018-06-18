---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Delete Alerts Policy Channels. Format
  version: 1.0.0
  description: "This API endpoint deletes Alerts policy/channel associations.\n\nNote:
    Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
    on deleting notification channels with policies."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_policy_channels.{format}:
    put:
      summary: Put Alerts Policy Channels. Format
      description: "This API endpoint updates policy/channel associations.\n\nNote:
        Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
        on updating notification channels with policies."
      operationId: putAlertsPolicyChannels.Format
      x-api-path-slug: alerts-policy-channels-format-put
      parameters:
      - in: query
        name: channel_ids
        description: Channel IDs
        type: list
      - in: query
        name: policy_id
        description: Policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Policy
      - Channels.
      - Format
    delete:
      summary: Delete Alerts Policy Channels. Format
      description: "This API endpoint deletes Alerts policy/channel associations.\n\nNote:
        Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
        on deleting notification channels with policies."
      operationId: deleteAlertsPolicyChannels.Format
      x-api-path-slug: alerts-policy-channels-format-delete
      parameters:
      - in: query
        name: channel_id
        description: Channel ID
        type: integer
      - in: query
        name: policy_id
        description: Policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Policy
      - Channels.
      - Format
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