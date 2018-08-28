---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Enable Sso
  version: 1.0.0
  description: Enables single sign-on for a directory.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableRadius:
    get:
      summary: Enable Radius
      description: Enables multi-factor authentication (MFA) with the Remote Authentication
        Dial In User Service (RADIUS) server for an AD Connector directory.
      operationId: enableRadius
      x-api-path-slug: actionenableradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to enable MFA
        type: string
      - in: query
        name: RadiusSettings
        description: A RadiusSettings object that contains information about the RADIUS
          server
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
  /?Action=EnableSso:
    get:
      summary: Enable Sso
      description: Enables single sign-on for a directory.
      operationId: enableSso
      x-api-path-slug: actionenablesso-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to enable single-sign
          on
        type: string
      - in: query
        name: Password
        description: The password of an alternate account to use to enable single-sign
          on
        type: string
      - in: query
        name: UserName
        description: The username of an alternate account to use to enable single-sign
          on
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSO
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