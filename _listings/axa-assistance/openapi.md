swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 1
info:
  title: AXA Assistance
  description: axa-assistance-is-a-worldwide-specialist-for-car-insurance-travel-health-and-home-services--trust-in-axa-assistance-for-your-insurance
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/v1/identities/{identity_id}/channels/confirm:
    post:
      summary: Confirm channels
      description: Confirm channels
      operationId: postUserV1IdentitiesIdentity_idChannelsConfirm
      x-api-path-slug: userv1identitiesidentity-idchannelsconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: identity_id
        description: ID of the identity
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Confirm
      - channels
  /user/v1/identities/{identity_id}/channels/sms:
    get:
      summary: Get channel
      description: Get channel
      operationId: getUserV1IdentitiesIdentity_idChannelsSms
      x-api-path-slug: userv1identitiesidentity-idchannelssms-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - channel
    put:
      summary: Update channel
      description: Update channel
      operationId: putUserV1IdentitiesIdentity_idChannelsSms
      x-api-path-slug: userv1identitiesidentity-idchannelssms-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: identity_id
        description: ID of the identity
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - channel
  /user/v1/identities/{identity_id}/channels/email:
    put:
      summary: Update channel
      description: Update channel
      operationId: putUserV1IdentitiesIdentity_idChannelsEmail
      x-api-path-slug: userv1identitiesidentity-idchannelsemail-put
      parameters:
      - in: path
        name: identity_id
        description: ID of the identity
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - channel