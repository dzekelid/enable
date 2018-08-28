---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Enable a discount
  description: Enable a discount.
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
  /admin/discounts/2951196163/enable.json:
    post:
      summary: Enable a discount
      description: Enable a discount.
      operationId: postAdminDiscounts2951196163Enable.json
      x-api-path-slug: admindiscounts2951196163enable-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Enable
      - Discount
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