swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/offchain/channelkey:
    get:
      summary: Get API Offchain Channelkey
      description: Get api offchain channelkey.
      operationId: ApiOffchainChannelkeyGet
      x-api-path-slug: apioffchainchannelkey-get
      parameters:
      - in: query
        name: asset
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Channelkey