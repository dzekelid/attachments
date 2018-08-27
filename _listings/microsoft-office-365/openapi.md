swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 1
info:
  title: Microsoft Office 365
  description: office-365-is-the-brand-name-used-by-microsoft-for-a-group-of-software-plus-services-subscriptions-that-provides-productivity-software-and-related-services-to-its-subscribers-
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
    delete:
      summary: Delete Contacts Contact Attachments
      description: To delete an attachment, send a DELETE request to the URL of...
      operationId: deleteContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-delete
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
    parameters:
      summary: Parameters Contacts Contact Attachments
      description: Parameters contacts contact  attachments
      operationId: parametersContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-parameters
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments