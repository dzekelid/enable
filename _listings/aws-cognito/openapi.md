swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminEnableUser:
    get:
      summary: Admin Enable User
      description: Enables the specified user as an administrator.
      operationId: adminEnableUser
      x-api-path-slug: actionadminenableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to enable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to enable the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users