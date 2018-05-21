---
swagger: "2.0"
x-collection-name: Google Adsense
x-complete: 0
info:
  title: Google Adsense API Delete URL Channel
  version: 1.0.0
  description: Delete a URL channel from the host AdSense account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /adclients/{adClientId}/customchannels:
    get:
      summary: Get Custom Channels
      description: List all host custom channels in this AdSense account.
      operationId: adsensehost.customchannels.list
      x-api-path-slug: adclientsadclientidcustomchannels-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client for which to list custom channels
      - in: query
        name: maxResults
        description: The maximum number of custom channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through custom channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    patch:
      summary: Update Custom Channels
      description: Update a custom channel in the host AdSense account. This method
        supports patch semantics.
      operationId: adsensehost.customchannels.patch
      x-api-path-slug: adclientsadclientidcustomchannels-patch
      parameters:
      - in: path
        name: adClientId
        description: Ad client in which the custom channel will be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: customChannelId
        description: Custom channel to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    post:
      summary: Create Custom Channels
      description: Add a new custom channel to the host AdSense account.
      operationId: adsensehost.customchannels.insert
      x-api-path-slug: adclientsadclientidcustomchannels-post
      parameters:
      - in: path
        name: adClientId
        description: Ad client to which the new custom channel will be added
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    put:
      summary: Update Custom Channel
      description: Update a custom channel in the host AdSense account.
      operationId: adsensehost.customchannels.update
      x-api-path-slug: adclientsadclientidcustomchannels-put
      parameters:
      - in: path
        name: adClientId
        description: Ad client in which the custom channel will be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/customchannels/{customChannelId}:
    delete:
      summary: Delete Custom Channel
      description: Delete a specific custom channel from the host AdSense account.
      operationId: adsensehost.customchannels.delete
      x-api-path-slug: adclientsadclientidcustomchannelscustomchannelid-delete
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to delete the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    get:
      summary: Get Custom Channel
      description: Get a specific custom channel from the host AdSense account.
      operationId: adsensehost.customchannels.get
      x-api-path-slug: adclientsadclientidcustomchannelscustomchannelid-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to get the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/urlchannels:
    get:
      summary: Get URL Channels
      description: List all host URL channels in the host AdSense account.
      operationId: adsensehost.urlchannels.list
      x-api-path-slug: adclientsadclientidurlchannels-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client for which to list URL channels
      - in: query
        name: maxResults
        description: The maximum number of URL channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through URL channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    post:
      summary: Add URL Channel
      description: Add a new URL channel to the host AdSense account.
      operationId: adsensehost.urlchannels.insert
      x-api-path-slug: adclientsadclientidurlchannels-post
      parameters:
      - in: path
        name: adClientId
        description: Ad client to which the new URL channel will be added
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/urlchannels/{urlChannelId}:
    delete:
      summary: Delete URL Channel
      description: Delete a URL channel from the host AdSense account.
      operationId: adsensehost.urlchannels.delete
      x-api-path-slug: adclientsadclientidurlchannelsurlchannelid-delete
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to delete the URL channel
      - in: path
        name: urlChannelId
        description: URL channel to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
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