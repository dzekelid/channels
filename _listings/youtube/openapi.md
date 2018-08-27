swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels:
    get:
      summary: Get Channels
      description: Returns a collection of zero or more channel resources that match
        the request criteria.
      operationId: getChannels
      x-api-path-slug: channels-get
      parameters:
      - in: query
        name: categoryId
        description: The categoryId parameter specifies a YouTube guide category,
          thereby requesting YouTube channels associated with that category
      - in: query
        name: forUsername
        description: The forUsername parameter specifies a YouTube username, thereby
          requesting the channel associated with that username
      - in: query
        name: hl
        description: The hl parameter should be used for filter out the properties
          that are not in the given language
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channel ID(s) for the resource(s) that are being retrieved
      - in: query
        name: managedByMe
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return channels owned by the authenticated user
      - in: query
        name: mySubscribers
        description: Use the subscriptions
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more channel resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Channels
    put:
      summary: Put Channels
      description: Updates a channel's metadata. Note that this method currently only
        supports updates to the channel resource's brandingSettings and invideoPromotion
        objects and their child properties.
      operationId: putChannels
      x-api-path-slug: channels-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: The onBehalfOfContentOwner parameter indicates that the authenticated
          user is acting on behalf of the content owner specified in the parameter
          value
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Channels
  /channelBanners/insert:
    post:
      summary: Add Channel Banners Insert
      description: |-
        Uploads a channel banner image to YouTube. This method represents the first two steps in a three-step process to update the banner image for a channel:

        - Call the channelBanners.insert method to upload the binary image data to YouTube. The image must have a 16:9 aspect ratio and be at least 2120x1192 pixels.
        - Extract the url property's value from the response that the API returns for step 1.
        - Call the channels.update method to update the channel's branding settings. Set the brandingSettings.image.bannerExternalUrl property's value to the URL obtained in step 2.
      operationId: postChannelbannersInsert
      x-api-path-slug: channelbannersinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: channelId
        description: The channelId parameter identifies the YouTube channel to which
          the banner is uploaded
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Channelbanners
      - Insert