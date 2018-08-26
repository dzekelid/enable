---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableMetricsCollection:
    get:
      summary: Enable Metrics Collection
      description: Enables group metrics for the specified Auto Scaling group.
      operationId: enableMetricsCollection
      x-api-path-slug: actionenablemetricscollection-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or ARN of the Auto Scaling group
        type: string
      - in: query
        name: Granularity
        description: The granularity to associate with the metrics to collect
        type: string
      - in: query
        name: Metrics.member.N
        description: One or more of the following metrics
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics Collection
---