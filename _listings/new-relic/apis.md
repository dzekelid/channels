---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Channels
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Put Alerts Policy Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint updates policy/channel associations.\n\nNote: Admin
    User\u2019s API Key is required.\n\nSee our documentation for a discussion on
    updating notification channels with policies."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_policy_channels.{format}
  tags: Alerts, Policy, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-policy-channels-format-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-policy-channels-format-put-openapi.md
- name: New Relic Delete Alerts Policy Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint deletes Alerts policy/channel associations.\n\nNote:
    Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
    on deleting notification channels with policies."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_policy_channels.{format}
  tags: Alerts, Policy, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-policy-channels-format-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-policy-channels-format-delete-openapi.md
- name: New Relic Get Alerts Channels. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint works with new Alerts on alerts.newrelic.com.

    It returns a list of the channels associated with your New Relic account.

    See our documentation for a discussion on listing notification channels.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels.{format}
  tags: Alerts, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-channels-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-channels-format-get-openapi.md
- name: New Relic Add Alerts Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
    creates a channel associated with your New Relic account.\n\nNote: Admin User\u2019s
    API Key is required.\n\nSee our documentation for a discussion on creating notification
    channels.\n\nChannel type configuration options:\n\n\n  \n    Email\n\n    {\n\n
    \   \"recipients\" : \"test@google.com\",\n\"include_json_attachment\" : true\n\n\n
    \   }\n  \n  \n    HipChat\n\n    {\n\n    \"auth_token\": \"abc123\",\n\"room_id\":
    \"google.com\"\n\n\n    }\n  \n  \n    OpsGenie\n\n    {\n\n    \"api_key\": \"abc123\",\n\"teams\":
    \"team1\",\n\"tags\": \"tag1\",\n\"recipients\": \"me@me.com\"\n\n\n    }\n  \n
    \ \n    Slack\n\n    {\n\n    \"url\": \"http://test.com\",\n\"channel\": \"channel1\"\n\n\n
    \   }\n  \n  \n    Campfire\n\n    {\n\n    \"subdomain\": \"mysubdomain\",\n\"token\":
    \"123abc\",\n\"room\": \"room1\"\n\n\n    }\n  \n  \n    Victorops\n\n    {\n\n
    \   \"key\": \"mykey\",\n\"route_key\": \"theroute\"\n\n\n    }\n  \n  \n    PagerDuty\n\n
    \   {\n\n    \"service_key\": \"myservicekey\"\n\n\n    }\n  \n  \n    Webhook
    (json)\n\n    {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\":
    \"username\",\n\"auth_password\": \"password\",\n\"payload_type\": \"application/json\",\n\"payload\":
    {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
    \"test\", \"header2\": \"test\"}\n\n\n    }\n  \n  \n    Webhook (x-www-form-urlencoded)\n\n
    \   {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
    \"password\",\n\"payload_type\": \"application/x-www-form-urlencoded\",\n\"payload\":
    {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
    \"test\", \"header2\": \"test\"}\n\n\n    }"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels.{format}
  tags: Alerts, Channels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-channels-format-post-openapi.md
- name: New Relic Delete Alerts Channels Channel  . Format
  x-api-slug: new-relic
  description: "This API endpoint deletes Alerts notification channels.\n\nNote: Admin
    User\u2019s API Key is required.\n\nSee our documentation for a discussion on
    deleting notification channels."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels/{channel_id}.{format}
  tags: Alerts, Channels, Channel, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/alerts-channelschannel-id-format-delete-openapi.md
- name: New Relic Get Notification Channels. Format
  x-api-slug: new-relic
  description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
    API endpoint returns a paginated \nlist of the notification channels associated
    with your New Relic account.\n\nNotification channels can be filtered by their
    type or a list of IDs."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///notification_channels.{format}
  tags: Notification, Channels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/notification-channels-format-get-openapi.md
- name: New Relic Get Notification Channels  . Format
  x-api-slug: new-relic
  description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
    API endpoint returns a single notification channel, identified by ID.\u201D"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///notification_channels/{id}.{format}
  tags: Notification, Channels, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/notification-channelsid-format-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic???s digital intelligence platform lets developers, ops, and
    tech teams measure and monitor the performance of their applications and infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---