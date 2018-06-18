---
swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 0
info:
  title: Microsoft Office 365 Add Contacts Contact Attachments
  description: To add an attachment to an item, send a POST request to the ...
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Contacts{contact_id}/Attachments:
    get:
      summary: Get Contacts Contact Attachments
      description: To get attachments, send a GET request to the Attachments pr...
      operationId: getContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-get
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
    post:
      summary: Add Contacts Contact Attachments
      description: To add an attachment to an item, send a POST request to the ...
      operationId: postContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
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