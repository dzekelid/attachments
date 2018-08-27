swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 1
info:
  title: Elastic Email SMTP API
  description: api-for-sending-and-management-email-
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  attachments/upload/:
    get:
      summary: Upload Attachment
      description: The upload attachment command is used to upload an attachment for
        sending.
      operationId: getAttachmentsUpload
      x-api-path-slug: attachmentsupload-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: file
        description: The file name being uploaded
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Upload