swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutKeyPolicy:
    get:
      summary: Put Key Policy
      description: Attaches a key policy to the specified customer master key (CMK).
      operationId: putKeyPolicy
      x-api-path-slug: actionputkeypolicy-get
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      - in: query
        name: PolicyName
        description: The name of the key policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys