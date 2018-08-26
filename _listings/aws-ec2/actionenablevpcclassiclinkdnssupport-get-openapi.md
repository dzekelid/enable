---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Enable Vpc Classic Link Dns Support
  version: 1.0.0
  description: Enables a VPC to support DNS hostname resolution for ClassicLink.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnableVgwRoutePropagation:
    get:
      summary: Enable Vgw Route Propagation
      description: Enables a virtual private gateway (VGW) to propagate routes to
        the specified route table of a VPC.
      operationId: enablevgwroutepropagation
      x-api-path-slug: actionenablevgwroutepropagation-get
      parameters:
      - in: query
        name: DestinationCidrBlock
        description: The IPv4 CIDR address block used for the destination match
        type: string
      - in: query
        name: DestinationIpv6CidrBlock
        description: The IPv6 CIDR address block used for the destination match
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EgressOnlyInternetGatewayId
        description: '[IPv6 traffic only] The ID of an egress-only Internet gateway'
        type: string
      - in: query
        name: GatewayId
        description: The ID of an Internet gateway or virtual private gateway
        type: string
      - in: query
        name: InstanceId
        description: The ID of a NAT instance in your VPC
        type: string
      - in: query
        name: NatGatewayId
        description: '[IPv4 traffic only] The ID of a NAT gateway'
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of a network interface
        type: string
      - in: query
        name: RouteTableId
        description: The ID of the route table
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of a VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual Private Gateway Route Propogation
  /?Action=EnableVolumeIO:
    get:
      summary: Enable Volume I O
      description: |-
        Enables I/O operations for a volume that had I/O operations disabled because the data on the
              volume was potentially inconsistent.
      operationId: enablevolumeio
      x-api-path-slug: actionenablevolumeio-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute to modify
        type: string
      - in: query
        name: CreateVolumePermission
        description: A JSON representation of the snapshot attribute modification
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: OperationType
        description: The type of operation to perform to the attribute
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      - in: query
        name: UserGroup.N
        description: The group to modify for the snapshot
        type: string
      - in: query
        name: UserId.N
        description: The account ID to modify for the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /?Action=EnableVpcClassicLink:
    get:
      summary: Enable Vpc Classic Link
      description: Enables a VPC for ClassicLink.
      operationId: enablevpcclassiclink
      x-api-path-slug: actionenablevpcclassiclink-get
      parameters:
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=EnableVpcClassicLinkDnsSupport:
    get:
      summary: Enable Vpc Classic Link Dns Support
      description: Enables a VPC to support DNS hostname resolution for ClassicLink.
      operationId: enablevpcclassiclinkdnssupport
      x-api-path-slug: actionenablevpcclassiclinkdnssupport-get
      parameters:
      - in: query
        name: BgpAsn
        description: For devices that support BGP, the customer gateways BGP ASN
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: IpAddress
        description: The Internet-routable IP address for the customer gateways outside
          interface
        type: string
      - in: query
        name: Type
        description: The type of VPN connection that this customer gateway supports
          (ipsec
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC NS
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