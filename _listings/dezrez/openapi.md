---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branding/{id}/attachexternaldocument:
    put:
      summary: Attaches an external document to brand.
      description: Attaches an external document to brand..
      operationId: Branding_AttachExternalDocumentByidByexternalDocument
      x-api-path-slug: apibrandingidattachexternaldocument-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - External
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocument:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apibrandingiduploadandattachdocument-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocumenttodefault:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentToDefaultBrandBydocumentDetailsByid
      x-api-path-slug: apibrandingiduploadandattachdocumenttodefault-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/attachdocument:
    put:
      summary: Attaches a document to a brand.
      description: Attaches a document to a brand..
      operationId: Branding_AttachDocumentByidBydocumentId
      x-api-path-slug: apibrandingidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Document
      - To
      - Brand
  /api/group/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a group
      description: Attaches an existing document to a group.
      operationId: Group_AttachDocumentByidBydocumentId
      x-api-path-slug: apigroupidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the group to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Group
  /api/group/{id}/uploadandattachdocument:
    post:
      summary: Uploads a new document and attaches it to the specified group.
      description: Uploads a new document and attaches it to the specified group..
      operationId: Group_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apigroupiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Document
      - Attaches
      - It
      - To
      - Specified
      - Group
  /api/group/{id}/attachexternaldocument:
    post:
      summary: Attaches the external document.
      description: Attaches the external document..
      operationId: Group_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apigroupidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - External
      - Document
  /api/milestone/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a milestone
      description: Attaches an existing document to a milestone.
      operationId: Milestone_AttachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the milestone to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Milestone
  /api/property/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a property
      description: Attaches an existing document to a property.
      operationId: Property_AttachDocumentByidBydocumentId
      x-api-path-slug: apipropertyidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the property to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Property
  /api/property/{id}/attachexternaldocument:
    post:
      summary: Attaches an externally hosted document to a property
      description: Attaches an externally hosted document to a property.
      operationId: Property_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apipropertyidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: Details of the document to associate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Property
  /api/role/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a role
      description: Attaches an existing document to a role.
      operationId: Role_AttachDocumentByidBydocumentId
      x-api-path-slug: apiroleidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the role to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Role
  /api/role/{id}/attachexternaldocument:
    post:
      summary: Attaches an externally hosted document to a role
      description: Attaches an externally hosted document to a role.
      operationId: Role_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apiroleidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: Details of the document to associate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Role
  /api/roomdescription/{id}/attachexternaldocumenttoroom:
    put:
      summary: Attaches an externally hosted document to a room within a room description.
      description: Attaches an externally hosted document to a room within a room
        description..
      operationId: RoomDescription_AttachExternalDocumentToRoomByidByexternalDocumentByroomId
      x-api-path-slug: apiroomdescriptionidattachexternaldocumenttoroom-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The RoomDescriptionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room identifier
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Room
      - Within
      - Room
      - Description
  /api/roomdescription/{id}/uploadandattachdocumenttoroom:
    put:
      summary: Uploads and attaches a document to room description room - the new
        document is appended to the current list.
      description: Uploads and attaches a document to room description room - the
        new document is appended to the current list..
      operationId: RoomDescription_UploadAndAttachDocumentToRoomByidByroomIdBydocumentDetails
      x-api-path-slug: apiroomdescriptioniduploadandattachdocumenttoroom-put
      parameters:
      - in: body
        name: documentDetails
        description: Details about the document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The roomId
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Room
      - Description
      - Room
      - '-'
      - New
      - Document
      - Is
      - Appended
      - To
      - Current
      - List
  /api/roomdescription/{id}/attachdocumentoroom:
    put:
      summary: Attaches the document to room.
      description: Attaches the document to room..
      operationId: RoomDescription_AttachDocumentToRoomByidBydocumentIdByroomIdByinsertAtIndex
      x-api-path-slug: apiroomdescriptionidattachdocumentoroom-put
      parameters:
      - in: query
        name: documentId
        description: The document identifier
      - in: path
        name: id
        description: The identifier
      - in: query
        name: insertAtIndex
        description: Index of the insert at
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room identifier
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Document
      - To
      - Room
---