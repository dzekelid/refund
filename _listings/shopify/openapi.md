---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4554953422/refunds/646546.json:
    get:
      summary: Get a representation of a single refund
      description: Get a representation of a single refund.
      operationId: getAdminOrders4554953422Refunds646546.json
      x-api-path-slug: adminorders4554953422refunds646546-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Representation
      - Single
      - Refund
---