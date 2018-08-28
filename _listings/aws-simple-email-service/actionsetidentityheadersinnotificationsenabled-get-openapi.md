---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Set Identity Headers In Notifications Enabled
  version: 1.0.0
  description: "Given an identity (an email address or a domain), sets whether Amazon
    SES includes \n            the original email headers in the Amazon Simple Notification
    Service (Amazon SNS) notifications \n            of a specified type."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetIdentityDkimEnabled:
    get:
      summary: Set Identity Dkim Enabled
      description: |-
        Enables or disables Easy DKIM signing of email sent from an identity:If Easy DKIM
                    signing is enabled for a domain name identity (e.
      operationId: setIdentityDkimEnabled
      x-api-path-slug: actionsetidentitydkimenabled-get
      parameters:
      - in: query
        name: DkimEnabled
        description: Sets whether DKIM signing is enabled for an identity
        type: string
      - in: query
        name: Identity
        description: The identity for which DKIM signing should be enabled or disabled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=SetIdentityFeedbackForwardingEnabled:
    get:
      summary: Set Identity Feedback Forwarding Enabled
      description: Given an identity (an email address or a domain), enables or disables
        whether Amazon SES forwards bounce and complaint notifications as email.
      operationId: setIdentityFeedbackForwardingEnabled
      x-api-path-slug: actionsetidentityfeedbackforwardingenabled-get
      parameters:
      - in: query
        name: ForwardingEnabled
        description: Sets whether Amazon SES will forward bounce and complaint notifications
          as email
        type: string
      - in: query
        name: Identity
        description: The identity for which to set bounce and complaint notification
          forwarding
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=SetIdentityHeadersInNotificationsEnabled:
    get:
      summary: Set Identity Headers In Notifications Enabled
      description: "Given an identity (an email address or a domain), sets whether
        Amazon SES includes \n            the original email headers in the Amazon
        Simple Notification Service (Amazon SNS) notifications \n            of a
        specified type."
      operationId: setIdentityHeadersInNotificationsEnabled
      x-api-path-slug: actionsetidentityheadersinnotificationsenabled-get
      parameters:
      - in: query
        name: Enabled
        description: Sets whether Amazon SES includes the original email headers in
          Amazon SNS notifications             of the specified notification type
        type: string
      - in: query
        name: Identity
        description: The identity for which to enable or disable headers in notifications
        type: string
      - in: query
        name: NotificationType
        description: The notification type for which to enable or disable headers
          in notifications
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=SetIdentityMailFromDomain:
    get:
      summary: Set Identity Mail From Domain
      description: Enables or disables the custom MAIL FROM domain setup for a verified
        identity (an email address or a domain).
      operationId: setIdentityMailFromDomain
      x-api-path-slug: actionsetidentitymailfromdomain-get
      parameters:
      - in: query
        name: BehaviorOnMXFailure
        description: The action that you want Amazon SES to take if it cannot successfully
          read the required MX record when you send an email
        type: string
      - in: query
        name: Identity
        description: The verified identity for which you want to enable or disable
          the specified custom MAIL FROM domain
        type: string
      - in: query
        name: MailFromDomain
        description: The custom MAIL FROM domain that you want the verified identity
          to use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
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