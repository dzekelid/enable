---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Enable Snapshot Copy
  version: 1.0.0
  description: |-
    Enables the automatic copy of snapshots from one region to another region for a
                specified cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableLogging:
    get:
      summary: Enable Logging
      description: |-
        Starts logging information, such as queries and connection attempts, for the
                    specified Amazon Redshift cluster.
      operationId: enableLogging
      x-api-path-slug: actionenablelogging-get
      parameters:
      - in: query
        name: BucketName
        description: The name of an existing S3 bucket where the log files are to
          be stored
        type: string
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster on which logging is to be started
        type: string
      - in: query
        name: S3KeyPrefix
        description: The prefix applied to the log file names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging
  /?Action=EnableSnapshotCopy:
    get:
      summary: Enable Snapshot Copy
      description: |-
        Enables the automatic copy of snapshots from one region to another region for a
                    specified cluster.
      operationId: enableSnapshotCopy
      x-api-path-slug: actionenablesnapshotcopy-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster to copy snapshots
          from
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region that you want to copy snapshots to
        type: string
      - in: query
        name: RetentionPeriod
        description: The number of days to retain automated snapshots in the destination
          region after            they are copied from the source region
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to use when snapshots of
          an AWS KMS-encrypted            cluster are copied to the destination region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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