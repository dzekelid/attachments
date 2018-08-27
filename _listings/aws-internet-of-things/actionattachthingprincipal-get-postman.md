{
  "info": {
    "name": "AWS Internet of Things API Attach Thing Principal",
    "_postman_id": "566dad3e-dd54-4b16-9d7a-e296c0011c83",
    "description": "Attaches the specified principal to the specified thing.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Certificate Transfers",
      "item": [
        {
          "id": "8728ec8b-7f1f-450c-95f4-20ac2c7f997d",
          "name": "acceptCertificateTransfer",
          "request": {
            "url": "http://example.com/api/?Action=AcceptCertificateTransfer?certificateId=certificateId&setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a pending certificate transfer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bec4953-d960-449e-bc90-51ee7a843196"
            }
          ]
        }
      ]
    },
    {
      "name": "Principal Policies",
      "item": [
        {
          "id": "620e8e0f-3359-4fbb-9d52-0a5b92f63722",
          "name": "attachPrincipalPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachPrincipalPolicy?policyName=policyName&principal=principal",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified policy to the specified principal (certificate or other credential)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3304aed7-8236-42e2-9094-1041e73345d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Thing Principals",
      "item": [
        {
          "id": "d998f9e9-ceee-4b29-a8a6-106c53d55efc",
          "name": "attachThingPrincipal",
          "request": {
            "url": "http://example.com/api/?Action=AttachThingPrincipal?principal=principal&thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified principal to the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c44a604-5810-4e58-8a80-e770d1cfb86a"
            }
          ]
        }
      ]
    }
  ]
}