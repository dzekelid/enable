---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableTopicRule:
    get:
      summary: Enable Topic Rule
      description: Enables the specified rule.
      operationId: enableTopicRule
      x-api-path-slug: actionenabletopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the topic rule to enable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
---