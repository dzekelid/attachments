---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Upload an attachment
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Attachments:
    get:
      summary: Get a list of all attachments matching a given filter.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_GetList
      x-api-path-slug: apiv1attachments-get
      parameters:
      - in: query
        name: acknowledged
        description: Acknowledged flag
      - in: query
        name: logicbrokerKey
        description: Logicbroker key
      - in: query
        name: page
        description: Page number
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Attachments
      - Matching
      - Given
      - Filter
    post:
      summary: Upload an attachment
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_Upload
      x-api-path-slug: apiv1attachments-post
      parameters:
      - in: body
        name: data
        description: XML/JSON data to attach (webhooks)
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: description
        description: Attachment description
      - in: formData
        name: file
        description: File to attach
      - in: query
        name: logicbrokerKey
        description: Logicbroker key to attach
      - in: query
        name: notify
        description: If true, create an activty event
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type (json, xml, csv, txt, pdf, png)
      - in: query
        name: url
        description: URL of file to attach
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Attachment
  /api/v1/Attachments/{container}/{name}:
    get:
      summary: Retrieve a file from Logicbroker storage.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_DownloadWithCoId
      x-api-path-slug: apiv1attachmentscontainername-get
      parameters:
      - in: path
        name: container
        description: File container (ex
      - in: path
        name: name
        description: File name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - File
      - From
      - Logicbroker
      - Storage
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