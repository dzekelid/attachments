---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /attachments/{id}:
    delete:
      summary: Delete attachment
      description: Delete attachment.
      operationId: attachments.id.delete
      x-api-path-slug: attachmentsid-delete
      parameters:
      - in: path
        name: id
        description: Attachment id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Attachment
  /maps/{id}/attachments:
    post:
      summary: Upload map attachment
      description: Upload map attachment. Wrap attachment parameters in [attachment]
      operationId: maps.id.attachments.post
      x-api-path-slug: mapsidattachments-post
      parameters:
      - in: path
        name: id
        description: Map id
      - in: body
        name: image
        description: Base64 encoded image
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Upload
      - Map
      - Attachment
    get:
      summary: List attachments for a given map
      description: List attachments for a given map.
      operationId: maps.id.attachments.get
      x-api-path-slug: mapsidattachments-get
      parameters:
      - in: path
        name: id
        description: Map id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Attachmentsa
      - Given
      - Map
  /spots/{id}/attachments:
    post:
      summary: Upload spot attachment
      description: Upload spot attachment. Wrap attachment parameters in [attachment]
      operationId: spots.id.attachments.post
      x-api-path-slug: spotsidattachments-post
      parameters:
      - in: path
        name: id
        description: Spot id
      - in: body
        name: image
        description: Base64 encoded image
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Upload
      - Spot
      - Attachment
    get:
      summary: List attachments for a given spot
      description: List attachments for a given spot.
      operationId: spots.id.attachments.get
      x-api-path-slug: spotsidattachments-get
      parameters:
      - in: path
        name: id
        description: Spot id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Attachmentsa
      - Given
      - Spot
---