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
  /api/RefundAddress:
    get:
      summary: Get API Refundaddress
      description: Get api refundaddress.
      operationId: ApiRefundAddressGet
      x-api-path-slug: apirefundaddress-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
    post:
      summary: Add API Refundaddress
      description: Add api refundaddress.
      operationId: ApiRefundAddressPost
      x-api-path-slug: apirefundaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: refundAddressModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
  /api/RefundSettings:
    get:
      summary: Get API Refundsettings
      description: Get api refundsettings.
      operationId: ApiRefundSettingsGet
      x-api-path-slug: apirefundsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundsettings
    post:
      summary: Add API Refundsettings
      description: Add api refundsettings.
      operationId: ApiRefundSettingsPost
      x-api-path-slug: apirefundsettings-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: refundAddressModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refundsettings