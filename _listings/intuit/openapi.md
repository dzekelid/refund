swagger: "2.0"
x-collection-name: Intuit
x-complete: 1
info:
  title: QuickBooks Online V3 API
  description: the-quickbooks-online-accounting-api-is-a-restful-api-that-is-used-to-access-quickbooks-companies-docs-
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /refundreceipt:
    post:
      summary: Post Refund Receipt
      description: |-
        Update a refund-receipt object
        Method : POST
      operationId: postRefundreceipt
      x-api-path-slug: refundreceipt-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Refund
      - Receipt
  /refundreceipt/66:
    get:
      summary: Get Refund Receipt
      description: |-
        Read a refund-receipt object
        Method : GET
      operationId: getRefundreceipt66
      x-api-path-slug: refundreceipt66-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Refund
      - Receipt