---
name: Slack
x-slug: slack
description: Slack is a team communication application providing services such as
  real-time messaging, archiving, and to search for modern teams. It offers one-on-one
  messaging, private groups, persistent chat rooms, and direct messaging as well as
  group chats organized by topic. All content inside Slack is searchable from one
  search box and it integrates with a number of third-party services, including Google
  Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Channels
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/apis.md
specificationVersion: "0.14"
apis:
- name: Slack - Archive Channel
  x-api-slug: channels-archive-post
  description: Archives a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-archive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-archive-post-openapi.md
- name: Slack - Get Channel
  x-api-slug: channels-info-get
  description: Gets information about a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-info-get-openapi.md
- name: Slack - Remove User From Channel
  x-api-slug: channels-kick-post
  description: Removes a user from a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-kick-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-kick-post-openapi.md
- name: Slack - Get Channel History
  x-api-slug: channels-history-get
  description: Fetches history of messages and events from a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-history-get-openapi.md
- name: Slack - Leave Channel
  x-api-slug: channels-leave-post
  description: Leaves a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-leave-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-leave-post-openapi.md
- name: Slack - Rename Channel
  x-api-slug: channels-rename-post
  description: Renames a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-rename-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-rename-post-openapi.md
- name: Slack - Mark Channel
  x-api-slug: channels-mark-post
  description: Sets the read cursor in a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-mark-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-mark-post-openapi.md
- name: Slack - Unarchive Channel
  x-api-slug: channels-unarchive-post
  description: Unarchives a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-unarchive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-unarchive-post-openapi.md
- name: Slack - Create Channel
  x-api-slug: channels-create-post
  description: Creates a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-create-post-openapi.md
- name: Slack - Join Channel
  x-api-slug: channels-join-post
  description: Joins a channel, creating it if needed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-join-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-join-post-openapi.md
- name: Slack - Set Channel Topic
  x-api-slug: channels-settopic-post
  description: Sets the topic for a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-settopic-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-settopic-post-openapi.md
- name: Slack - Set Channel Purpose
  x-api-slug: channels-setpurpose-post
  description: Sets the purpose for a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-setpurpose-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-setpurpose-post-openapi.md
- name: Slack - List Channels
  x-api-slug: channels-list-get
  description: Lists all channels in a Slack team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-list-get-openapi.md
- name: Slack - Invite Channel User
  x-api-slug: channels-invite-post
  description: Invites a user to a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-invite-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-invite-post-openapi.md
- name: Slack - Get Channel Thread
  x-api-slug: channels-replies-get
  description: Retrieve a thread of messages posted to a channel
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Collaboration, My API Stack, Indie EdTech Data Jam, Imports, Getting Started
    Example, Communications, Change Log Example, Stack Network, Stack, Media, Chats,
    Messages, Messages, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-replies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/slack/channels-replies-get-openapi.md
x-common:
- type: x-website
  url: https://api.slack.com
- type: x-api-gallery
  url: http://site24x7.api.gallery.streamdata.io
- type: x-api-stack
  url: http://slack.stack.network
- type: x-application-gallery
  url: https://slack.com/apps
- type: x-blog
  url: http://slackhq.com/
- type: x-blog
  url: https://medium.com/slack-developer-blog
- type: x-blog-rss
  url: http://slackhq.com/rss
- type: x-blog-rss
  url: https://medium.com/feed/slack-developer-blog
- type: x-branding
  url: https://slack.com/brand-guidelines
- type: x-buttons
  url: https://api.slack.com/docs/slack-button
- type: x-c-sharp-sdk
  url: https://api.slack.com/web
- type: x-change-log
  url: https://api.slack.com/changelog
- type: x-developer
  url: https://api.slack.com/
- type: x-faq
  url: https://api.slack.com/faq
- type: x-getting-started
  url: https://slack.com/getting-started
- type: x-github
  url: https://github.com/slackhq
- type: x-incoming-webhooks
  url: https://api.slack.com/incoming-webhooks
- type: x-oauth-overview
  url: https://api.slack.com/docs/oauth
- type: x-oauth-scopes
  url: https://api.slack.com/docs/oauth-scopes
- type: x-outgoing-webhooks
  url: https://api.slack.com/outgoing-webhooks
- type: x-presence
  url: https://api.slack.com/docs/presence
- type: x-pricing
  url: https://slack.com/pricing
- type: x-privacy
  url: https://slack.com/privacy-policy
- type: x-rate-limits
  url: https://api.slack.com/docs/rate-limits
- type: x-real-time-messaging-api
  url: https://api.slack.com/rtm
- type: x-road-map
  url: https://api.slack.com/roadmap
- type: x-security
  url: https://slack.com/security
- type: x-status
  url: https://status.slack.com/
- type: x-support
  url: https://get.slack.help/hc/en-us
- type: x-terms-of-service
  url: https://slack.com/terms-of-service
- type: x-transparency-report
  url: https://slack.com/transparency-report
- type: x-twitter
  url: https://twitter.com/slackapi
- type: x-website
  url: http://slack.com
- type: x-website
  url: https://slack.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---