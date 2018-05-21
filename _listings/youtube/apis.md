---
name: YouTube
x-slug: youtube
description: YouTube allows billions of people to discover, watch and share originally-created
  videos. YouTube provides a forum for people to connect, inform, and inspire others
  across the globe and acts as a distribution platform for original content creators
  and advertisers large and small.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Channels
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/apis.md
specificationVersion: "0.14"
apis:
- name: Youtube Delete Channel Sections
  x-api-slug: youtube
  description: Deletes a channelSection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channelSections
  tags: Channelsections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-delete-openapi.md
- name: Youtube Get Channel Sections
  x-api-slug: youtube
  description: Returns channelSection resources that match the API request criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channelSections
  tags: Channelsections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-get-openapi.md
- name: Youtube Parameters Channel Sections
  x-api-slug: youtube
  description: Parameters channelsections
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channelSections
  tags: Channelsections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-parameters-openapi.md
- name: Youtube Add Channel Sections
  x-api-slug: youtube
  description: Adds a channelSection for the authenticated user's channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channelSections
  tags: Channelsections
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-post-openapi.md
- name: Youtube Put Channel Sections
  x-api-slug: youtube
  description: Update a channelSection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channelSections
  tags: Channelsections
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channelsections-put-openapi.md
- name: Youtube Get Channels
  x-api-slug: youtube
  description: Returns a collection of zero or more channel resources that match the
    request criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channels
  tags: Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channels-get-openapi.md
- name: Youtube Parameters Channels
  x-api-slug: youtube
  description: Parameters channels
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channels
  tags: Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channels-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channels-parameters-openapi.md
- name: Youtube Put Channels
  x-api-slug: youtube
  description: Updates a channel's metadata. Note that this method currently only
    supports updates to the channel resource's brandingSettings and invideoPromotion
    objects and their child properties.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//channels
  tags: Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/channels-put-openapi.md
- name: Youtube
  x-api-slug: youtube
  description: YouTube allows billions of people to discover, watch and share originally-created
    videos. YouTube provides a forum for people to connect, inform, and inspire others
    across the globe and acts as a distribution platform for original content creators
    and advertisers large and small.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/youtube-logo.png
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1
  tags: Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/youtube/openapi.md
x-common:
- type: x-articles
  url: https://developers.google.com/youtube/articles/
- type: x-authentication
  url: https://developers.google.com/youtube/v3/guides/authentication
- type: x-blog
  url: https://youtube-eng.googleblog.com/
- type: x-blog-rss
  url: https://youtube-eng.googleblog.com/feeds/posts/default?alt=rss
- type: x-branding
  url: https://developers.google.com/youtube/branding_guidelines
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/entry
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/list?q=label:API-YouTube
- type: x-buttons
  url: https://developers.google.com/youtube/youtube_subscribe_button
- type: x-deprecation-policy
  url: https://developers.google.com/youtube/youtube-api-list
- type: x-developer
  url: https://developers.google.com/youtube/
- type: x-getting-started
  url: https://developers.google.com/youtube/v3/getting-started
- type: x-github
  url: https://github.com/youtube
- type: x-github
  url: https://github.com/youtube/
- type: x-terms-of-service
  url: https://developers.google.com/youtube/terms
- type: x-training
  url: https://developers.google.com/youtube/training/
- type: x-twitter
  url: https://twitter.com/YouTubeDev
- type: x-website
  url: https://www.youtube.com/
- type: x-widgets
  url: https://developers.google.com/youtube/youtube_upload_widget
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---