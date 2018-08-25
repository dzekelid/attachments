---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachInternetGateway:
    get:
      summary: Attach Internet Gateway
      description: "Attaches an Internet gateway to a VPC, enabling connectivity between
        the Internet\n\t\t\t\tand the VPC."
      operationId: attachinternetgateway
      x-api-path-slug: actionattachinternetgateway-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC for which to create the egress-only Internet
          gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=AttachNetworkInterface:
    get:
      summary: Attach Network Interface
      description: Attaches a network interface to an instance.
      operationId: attachnetworkinterface
      x-api-path-slug: actionattachnetworkinterface-get
      parameters:
      - in: query
        name: Description
        description: A description for the network interface
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Ipv6AddressCount
        description: The number of IPv6 addresses to assign to a network interface
        type: string
      - in: query
        name: Ipv6Addresses.N
        description: One or more specific IPv6 addresses from the IPv6 CIDR block
          range of your subnet
        type: string
      - in: query
        name: PrivateIpAddress
        description: The primary private IPv4 address of the network interface
        type: string
      - in: query
        name: PrivateIpAddresses.N
        description: One or more private IPv4 addresses
        type: string
      - in: query
        name: SecondaryPrivateIpAddressCount
        description: The number of secondary private IPv4 addresses to assign to a
          network interface
        type: string
      - in: query
        name: SecurityGroupId.N
        description: The IDs of one or more security groups
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet to associate with the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=AttachVolume:
    get:
      summary: Attach Volume
      description: |-
        Attaches an EBS volume to a running or stopped instance and exposes it to the instance with
              the specified device name.
      operationId: attachvolume
      x-api-path-slug: actionattachvolume-get
      parameters:
      - in: query
        name: Description
        description: A description for the EBS snapshot
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region to use in the PresignedUrl parameter of
          a snapshot copy      operation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the destination snapshot should be encrypted
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) CMK
          to use when creating the snapshot copy
        type: string
      - in: query
        name: PresignedUrl
        description: The pre-signed URL that facilitates copying an encrypted snapshot
        type: string
      - in: query
        name: SourceRegion
        description: The ID of the region that contains the snapshot to be copied
        type: string
      - in: query
        name: SourceSnapshotId
        description: The ID of the EBS snapshot to copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive Volume
  /?Action=AttachVpnGateway:
    get:
      summary: Attach Vpn Gateway
      description: Attaches a virtual private gateway to a VPC.
      operationId: attachvpngateway
      x-api-path-slug: actionattachvpngateway-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the virtual private gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Type
        description: The type of VPN connection this virtual private gateway supports
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPN Gateway
---