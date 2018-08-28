swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 1
info:
  title: AWS Shield API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateProtection:
    get:
      summary: Create Protection
      description: Enables AWS Shield Advanced for a specific AWS resource.
      operationId: createProtection
      x-api-path-slug: actioncreateprotection-get
      parameters:
      - in: query
        name: Name
        description: Friendly name for the Protection you are creating
        type: string
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection