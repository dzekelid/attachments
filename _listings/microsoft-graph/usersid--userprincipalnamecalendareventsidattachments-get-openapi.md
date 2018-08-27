---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Attachments
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: memailfoldersidchildfoldersid---messagesidattachmentsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamemailfoldersidchildfoldersidmessagesidattachmentsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: meeventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnameeventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /groups/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: groupsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendar/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: mecalendareventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/calendar/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamecalendareventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
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