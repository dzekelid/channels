---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_channels/{channel_id}.{format}:
    delete:
      summary: Delete Alerts Channels Channel  . Format
      description: |-
        This API endpoint deletes Alerts notification channels.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on deleting notification channels.
      operationId: deleteAlertsChannelsChannel.Format
      x-api-path-slug: alerts-channelschannel-id-format-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels
      - Channel
      - ""
      - .
      - Format
  /notification_channels/{id}.{format}:
    get:
      summary: Get Notification Channels  . Format
      description: |-
        WARNING: This is legacy alerting.  This endpoint will be deprecated.

        This API endpoint returns a single notification channel, identified by ID.???
      operationId: getNotificationChannels.Format
      x-api-path-slug: notification-channelsid-format-get
      parameters:
      - in: path
        name: id
        description: Notification Channel ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Channels
      - ""
      - .
      - Format
  /alerts_policy_channels.{format}:
    put:
      summary: Put Alerts Policy Channels. Format
      description: |-
        This API endpoint updates policy/channel associations.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on updating notification channels with policies.
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
      description: |-
        This API endpoint deletes Alerts policy/channel associations.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on deleting notification channels with policies.
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
  /alerts_channels.{format}:
    get:
      summary: Get Alerts Channels. Format
      description: |-
        This API endpoint works with new Alerts on alerts.newrelic.com.

        It returns a list of the channels associated with your New Relic account.

        See our documentation for a discussion on listing notification channels.
      operationId: getAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
    post:
      summary: Add Alerts Channels. Format
      description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
        creates a channel associated with your New Relic account.\n\nNote: Admin User???s
        API Key is required.\n\nSee our documentation for a discussion on creating
        notification channels.\n\nChannel type configuration options:\n\n\n  \n    Email\n\n
        \   {\n\n    \"recipients\" : \"test@google.com\",\n\"include_json_attachment\"
        : true\n\n\n    }\n  \n  \n    HipChat\n\n    {\n\n    \"auth_token\": \"abc123\",\n\"room_id\":
        \"google.com\"\n\n\n    }\n  \n  \n    OpsGenie\n\n    {\n\n    \"api_key\":
        \"abc123\",\n\"teams\": \"team1\",\n\"tags\": \"tag1\",\n\"recipients\": \"me@me.com\"\n\n\n
        \   }\n  \n  \n    Slack\n\n    {\n\n    \"url\": \"http://test.com\",\n\"channel\":
        \"channel1\"\n\n\n    }\n  \n  \n    Campfire\n\n    {\n\n    \"subdomain\":
        \"mysubdomain\",\n\"token\": \"123abc\",\n\"room\": \"room1\"\n\n\n    }\n
        \ \n  \n    Victorops\n\n    {\n\n    \"key\": \"mykey\",\n\"route_key\":
        \"theroute\"\n\n\n    }\n  \n  \n    PagerDuty\n\n    {\n\n    \"service_key\":
        \"myservicekey\"\n\n\n    }\n  \n  \n    Webhook (json)\n\n    {\n\n    \"base_url\":
        \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/json\",\n\"payload\": {\"account_id\":
        1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\": \"test\",
        \"header2\": \"test\"}\n\n\n    }\n  \n  \n    Webhook (x-www-form-urlencoded)\n\n
        \   {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/x-www-form-urlencoded\",\n\"payload\":
        {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
        \"test\", \"header2\": \"test\"}\n\n\n    }"
      operationId: postAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-post
      parameters:
      - in: body
        name: channel
        description: channel schema
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: policy_ids
        description: Policy IDs to associate with channel
        type: array
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
  /notification_channels.{format}:
    get:
      summary: Get Notification Channels. Format
      description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
        API endpoint returns a paginated \nlist of the notification channels associated
        with your New Relic account.\n\nNotification channels can be filtered by their
        type or a list of IDs."
      operationId: getNotificationChannels.Format
      x-api-path-slug: notification-channels-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by notification channel IDs
        type: list
      - in: query
        name: filter[type]
        description: Filter by notification channel types
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Channels.
      - Format
---