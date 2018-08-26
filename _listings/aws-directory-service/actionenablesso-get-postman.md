{
  "info": {
    "name": "AWS Directory Service API Enable Sso",
    "_postman_id": "96d34872-5c3a-4efd-80a5-c96d2d822c23",
    "description": "Enables single sign-on for a directory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "61f28fc9-dddd-4d79-9939-51932493c61e",
          "name": "addIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=AddIpRoutes?DirectoryId=DirectoryId&IpRoutes=IpRoutes&UpdateSecurityGroupForDirectoryControllers=UpdateSecurityGroupForDirectoryControllers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If the DNS server for your on-premises domain uses a publicly addressable IP address, you must add a CIDR address block to correctly route traffic to and from your Microsoft AD on Amazon Web Services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6fa7fd9-3c68-4c20-b133-9d5e06c63952"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "e6efe920-c90b-4bd6-b849-1e66c117754f",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e909bc52-9159-4a94-b229-f1d86a8a9357"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "e382b278-6e07-4b0d-89af-00cebf98392a",
          "name": "cancelSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=CancelSchemaExtension?DirectoryId=DirectoryId&SchemaExtensionId=SchemaExtensionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-progress schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0b885b5-d215-43b9-876e-1d3c4e2035b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "428ac791-9533-4466-9b05-f624aaba407f",
          "name": "connectDirectory",
          "request": {
            "url": "http://example.com/api/?Action=ConnectDirectory?ConnectSettings=ConnectSettings&Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AD Connector to connect to an on-premises directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8a65fb2-d62f-4cce-aa60-81f906c555ba"
            }
          ]
        },
        {
          "id": "e579163f-471b-4af9-9f3a-63dfd79f36a5",
          "name": "createDirectory",
          "request": {
            "url": "http://example.com/api/?Action=CreateDirectory?Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Simple AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "041be7a3-b190-4109-b569-6a44fc1ebc14"
            }
          ]
        },
        {
          "id": "a11b1d5e-9203-4325-a59a-d0b013a29f1e",
          "name": "deleteDirectory",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDirectory?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Directory Service directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3034c9d1-79ab-48e7-a95b-7b26eae6160f"
            }
          ]
        },
        {
          "id": "ccd979eb-3ae8-48fc-b78e-b7f8ae72eb89",
          "name": "describeDirectories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDirectories?DirectoryIds=DirectoryIds&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directories that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8870fac0-f2ec-4e30-bee1-177587fd3c97"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "6c0c0016-0fa3-46db-b860-1cd3e95ed10f",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?Alias=Alias&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for a directory and assigns the alias to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62526860-a40a-4c50-b977-ee469c532018"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "a6d767c9-c54d-4948-9f07-cd6f1b5b8362",
          "name": "createComputer",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputer?ComputerAttributes=ComputerAttributes&ComputerName=ComputerName&DirectoryId=DirectoryId&OrganizationalUnitDistinguishedName=OrganizationalUnitDistinguishedName&Password=Password",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a computer account in the specified directory, and joins the computer to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b17b36e8-8247-430e-be41-7218b6ac74db"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "423679ac-e30f-443f-bf34-20c0ecd8d54e",
          "name": "createConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=CreateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a conditional forwarder associated with your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69970db9-a8da-4083-8225-829e25470ef8"
            }
          ]
        },
        {
          "id": "c048bd91-0ebf-4b14-8cf0-d65d438b15f3",
          "name": "deleteConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConditionalForwarder?DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4848d66d-8413-4902-a467-482c5bf886ab"
            }
          ]
        },
        {
          "id": "a7c680ca-16c0-4fe7-9825-276c1975c967",
          "name": "describeConditionalForwarders",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConditionalForwarders?DirectoryId=DirectoryId&RemoteDomainNames=RemoteDomainNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the conditional forwarders for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00e36d00-c2c6-4fb6-9fc8-c4fe96de4145"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "0cb68838-e3a4-40c1-bfd4-7650ac55d6a1",
          "name": "createMicrosoftAD",
          "request": {
            "url": "http://example.com/api/?Action=CreateMicrosoftAD?Description=Description&Name=Name&Password=Password&ShortName=ShortName&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Microsoft AD in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40ff3125-f45b-4d5a-92ef-eb8806570f8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "2f0c51a5-bde5-452e-8fbf-3eb746d67688",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?DirectoryId=DirectoryId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c08d5c8-7c87-4300-852e-4be512e72b2e"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "36dadec0-1521-462e-9185-b41d8abaf0a5",
          "name": "createTrust",
          "request": {
            "url": "http://example.com/api/?Action=CreateTrust?ConditionalForwarderIpAddrs=ConditionalForwarderIpAddrs&DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName&TrustDirection=TrustDirection&TrustPassword=TrustPassword&TrustType=TrustType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AWS Directory Service for Microsoft Active Directory allows you to configure trust relationships."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e848ff8d-e93d-4106-b325-50434640577f"
            }
          ]
        },
        {
          "id": "33538e3c-c89d-45f8-993e-1df43b3a978a",
          "name": "deleteTrust",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTrust?DeleteAssociatedConditionalForwarder=DeleteAssociatedConditionalForwarder&TrustId=TrustId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing trust relationship between your Microsoft AD in the AWS cloud and an external domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bac3d10-bb0b-447e-8d10-d573d9aeb22e"
            }
          ]
        },
        {
          "id": "bf142037-6043-44e4-8279-cde98fc50513",
          "name": "describeTrusts",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTrusts?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&TrustIds=TrustIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the trust relationships for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0039ce29-bef0-4c74-88e8-b5083dd7a72e"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "34ce256e-a56e-401a-b662-43d1887e7d65",
          "name": "deleteSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1e21358-0a9b-4a01-b421-29f795242937"
            }
          ]
        },
        {
          "id": "28d78cc7-7d33-4530-bdaf-14ac317e8a24",
          "name": "describeSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshots?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&SnapshotIds=SnapshotIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directory snapshots that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96e29896-81f5-449c-9dfb-f7b1296c4a26"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "ab54c1c3-0370-4f28-a733-e88c790efd58",
          "name": "deregisterEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified directory as a publisher to the specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef17489d-c0b7-4c3c-966d-064fbd896e69"
            }
          ]
        },
        {
          "id": "3150c910-a0b6-414e-b201-1b2debc9ba32",
          "name": "describeEventTopics",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventTopics?DirectoryId=DirectoryId&TopicNames=TopicNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about which SNS topics receive status messages from the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "655113c2-f58b-472b-bf00-b325b90604bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "0239094e-d494-4906-92f8-fe4287910525",
          "name": "disableRadius",
          "request": {
            "url": "http://example.com/api/?Action=DisableRadius?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a14c3359-7039-4e20-9231-f3097c37fb36"
            }
          ]
        },
        {
          "id": "2166716a-a286-414f-bc16-9bdcf8b9c82a",
          "name": "enableRadius",
          "request": {
            "url": "http://example.com/api/?Action=EnableRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab741124-cc9f-4b6b-947e-b0ac7d06bfef"
            }
          ]
        }
      ]
    },
    {
      "name": "SSO",
      "item": [
        {
          "id": "a55c02bb-b5b5-4ac7-9ff4-e5d4b8694f2b",
          "name": "disableSso",
          "request": {
            "url": "http://example.com/api/?Action=DisableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables single-sign on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d8394e5-29b6-49d1-82b7-c48b120a9d75"
            }
          ]
        },
        {
          "id": "5804946b-6fd9-4e77-9fd3-2aa5300fb602",
          "name": "enableSso",
          "request": {
            "url": "http://example.com/api/?Action=EnableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables single sign-on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e9cf1be-05b5-4f8b-8cab-ba361c7dfeb7"
            }
          ]
        }
      ]
    }
  ]
}