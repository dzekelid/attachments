swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cards/{idCard}/attachments:
    get:
      summary: Get Cards Attachments
      description: Get cards attachments.
      operationId: getCardsAttachmentsByIdCard
      x-api-path-slug: cardsidcardattachments-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: filter
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
    post:
      summary: Post Cards Attachments
      description: Post cards attachments.
      operationId: addCardsAttachmentsByIdCard
      x-api-path-slug: cardsidcardattachments-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Attachments to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
  /cards/{idCard}/attachments/{idAttachment}:
    delete:
      summary: Delete Cards Attachments Attachment
      description: Delete cards attachments attachment.
      operationId: deleteCardsAttachmentsByIdCardByIdAttachment
      x-api-path-slug: cardsidcardattachmentsidattachment-delete
      parameters:
      - in: path
        name: idAttachment
        description: idAttachment
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
      - Attachment
    get:
      summary: Get Cards Attachments Attachment
      description: Get cards attachments attachment.
      operationId: getCardsAttachmentsByIdCardByIdAttachment
      x-api-path-slug: cardsidcardattachmentsidattachment-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: path
        name: idAttachment
        description: idAttachment
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
      - Attachment
  /cards/{idCard}/idAttachmentCover:
    put:
      summary: Put Cards Attachmentcover
      description: Put cards attachmentcover.
      operationId: updateCardsIdAttachmentCoverByIdCard
      x-api-path-slug: cardsidcardidattachmentcover-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Attachment Cover to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachmentcover