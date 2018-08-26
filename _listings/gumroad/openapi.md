---
swagger: "2.0"
x-collection-name: Gumroad
x-complete: 1
info:
  title: Gumroad
  description: api-for-selling-of-digital-goods-and-media-
  termsOfService: https://gumroad.com/terms
  version: v1
host: api.gumroad.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/:id/enable:
    put:
      summary: Put Products Enable
      description: Enable an existing product.
      operationId: putProductsEnable
      x-api-path-slug: productsidenable-put
      responses:
        200:
          description: OK
      tags:
      - Products
      - Enable
---