---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 1
info:
  title: Content API for Shopping
  description: manages-product-items-inventory-and-merchant-center-accounts-for-google-shopping-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{merchantId}/orders/{orderId}/refund:
    post:
      summary: Refund Order
      description: Refund a portion of the order, up to the full amount paid. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.refund
      x-api-path-slug: merchantidordersorderidrefund-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to refund
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Order
---