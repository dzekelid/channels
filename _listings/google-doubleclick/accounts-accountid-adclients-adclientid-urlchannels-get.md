---
swagger: "2.0"
info:
  title: Google Doubleclick API Get URL Channels
  version: 1.0.0
  description: List all URL channels in the specified ad client for this Ad Exchange
    account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/adclients/{adClientId}/urlchannels:
    get:
      summary: Get URL Channels
      description: List all URL channels in the specified ad client for this Ad Exchange
        account
      operationId: adexchangeseller.accounts.urlchannels.list
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
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
      - advertising
      - channels
definitions: []
x-collection-name: Google Doubleclick
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