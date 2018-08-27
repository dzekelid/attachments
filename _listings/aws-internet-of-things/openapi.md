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
  /?Action=AttachPrincipalPolicy:
    get:
      summary: Attach Principal Policy
      description: Attaches the specified policy to the specified principal (certificate
        or other credential).
      operationId: attachPrincipalPolicy
      x-api-path-slug: actionattachprincipalpolicy-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: principal
        description: The principal, which can be a certificate ARN (as returned from
          the CreateCertificate operation) or an Amazon Cognito ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
  /?Action=AttachThingPrincipal:
    get:
      summary: Attach Thing Principal
      description: Attaches the specified principal to the specified thing.
      operationId: attachThingPrincipal
      x-api-path-slug: actionattachthingprincipal-get
      parameters:
      - in: query
        name: principal
        description: The principal, such as a certificate or other credential
        type: string
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Principals