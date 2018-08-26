---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableKey:
    get:
      summary: Enable Key
      description: Marks a key as enabled, thereby permitting its use.
      operationId: enableKey
      x-api-path-slug: actionenablekey-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=EnableKeyRotation:
    get:
      summary: Enable Key Rotation
      description: Enables rotation of the specified customer master key.
      operationId: enableKeyRotation
      x-api-path-slug: actionenablekeyrotation-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
---