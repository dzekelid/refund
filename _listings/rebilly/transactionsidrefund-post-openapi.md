---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Refund a Transaction
  description: |-
    Refund a Transaction with specified identifier string.
    Note that the refund will be in the same currency as the original transaction.
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions/{id}/refund:
    post:
      summary: Refund a Transaction
      description: |-
        Refund a Transaction with specified identifier string.
        Note that the refund will be in the same currency as the original transaction.
      operationId: transactions.id.refund.post
      x-api-path-slug: transactionsidrefund-post
      parameters:
      - in: body
        name: body
        description: Transaction resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Transaction
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