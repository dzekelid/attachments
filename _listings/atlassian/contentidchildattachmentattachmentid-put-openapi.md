---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Update attachment properties
  description: "Updates the attachment properties, i.e. the non-binary data of an
    attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{id}/child/attachment:
    get:
      summary: Get attachments
      description: "Returns the attachments for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view the content. If the content is a blog post,
        'View' permission \nfor the space is required."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.getAttachments_get
      x-api-path-slug: contentidchildattachment-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the attachments
          to expand
      - in: query
        name: filename
        description: Filter the results to attachments that match the filename
      - in: path
        name: id
        description: The ID of the content to be queried for its attachments
      - in: query
        name: limit
        description: The maximum number of attachments to return per page
      - in: query
        name: mediaType
        description: Filter the results to attachments that match the media type
      - in: query
        name: start
        description: The starting index of the returned attachments
      responses:
        200:
          description: OK
      tags:
      - Attachments
    post:
      summary: Create attachment
      description: "Adds an attachment to a piece of content. This method only adds
        a new \nattachment. If you want to update an existing attachment, use \n[Create
        or update attachments](#api-content-id-child-attachment-put).\n\nNote, you
        must set a `X-Atlassian-Token: nocheck` header on the request \nfor this method,
        otherwise it will be blocked. This protects against XSRF \nattacks, which
        is necessary as this method accepts multipart/form-data.\n\nThe media type
        'multipart/form-data' is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt).
        \nMost client libraries have classes that make it easier to implement \nmultipart
        posts, like the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
        \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
        attaches a file ('example.txt') to a container \n(id='123') with a comment
        and `minorEdits`=true.\n\n``` bash\ncurl -D- \\\n  -u admin:admin \\\n  -X
        POST \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
        \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\"
        \\\n  http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.createAttachments_post
      x-api-path-slug: contentidchildattachment-post
      parameters:
      - in: path
        name: id
        description: The ID of the content to add the attachment to
      - in: query
        name: status
        description: The status of the content that the attachment is being added
          to
      responses:
        200:
          description: OK
      tags:
      - Attachment
    put:
      summary: Create or update attachment
      description: "Adds an attachment to a piece of content. If the attachment already
        exists \nfor the content, then the attachment is updated (i.e. a new version
        of the \nattachment is created).\n\nNote, you must set a `X-Atlassian-Token:
        nocheck` header on the request \nfor this method, otherwise it will be blocked.
        This protects against XSRF \nattacks, which is necessary as this method accepts
        multipart/form-data.\n\nThe media type 'multipart/form-data' is defined in
        [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client libraries
        have classes that make it easier to implement \nmultipart posts, like the
        [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
        \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
        attaches a file ('example.txt') to a piece of \ncontent (id='123') with a
        comment and `minorEdits`=true. If the 'example.txt' \nfile already exists,
        it will update it with a new version of the attachment.\n\n``` bash\ncurl
        -D- \\\n  -u admin:admin \\\n  -X PUT \\\n  -H \"X-Atlassian-Token: nocheck\"
        \\\n  -F \"file=@example.txt\" \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example
        attachment comment\" \\\n  http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.createOrUpdateAttachments_put
      x-api-path-slug: contentidchildattachment-put
      parameters:
      - in: path
        name: id
        description: The ID of the content to add the attachment to
      - in: query
        name: status
        description: The status of the content that the attachment is being added
          to
      responses:
        200:
          description: OK
      tags:
      - Update
      - Attachment
  /content/{id}/child/attachment/{attachmentId}:
    put:
      summary: Update attachment properties
      description: "Updates the attachment properties, i.e. the non-binary data of
        an attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.updateAttachmentProperties_put
      x-api-path-slug: contentidchildattachmentattachmentid-put
      parameters:
      - in: path
        name: attachmentId
        description: The ID of the attachment to update
      - in: path
        name: id
        description: The ID of the content that the attachment is attached to
      responses:
        200:
          description: OK
      tags:
      - Attachment
      - Properties
  /content/{id}/child/attachment/{attachmentId}/data:
    post:
      summary: Update attachment data
      description: "Updates the binary data of an attachment, given the attachment
        ID, and \noptionally the comment and the minor edit field.\n\nThis method
        is essentially the same as [Create or update attachments](#api-content-id-child-attachment-put),
        \nexcept that it matches the attachment ID rather than the name.\n\nNote,
        you must set a `X-Atlassian-Token: nocheck` header on the request \nfor this
        method, otherwise it will be blocked. This protects against XSRF \nattacks,
        which is necessary as this method accepts multipart/form-data.\n\nThe media
        type 'multipart/form-data' is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt).
        \nMost client libraries have classes that make it easier to implement \nmultipart
        posts, like the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
        \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
        updates an attachment (id='att456') that is attached  \nto a piece of content
        (id='123') with a comment and `minorEdits`=true. \n\n``` bash\ncurl -D- \\\n
        \ -u admin:admin \\\n  -X POST \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n
        \ -F \"file=@example.txt\" \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example
        attachment comment\" \\\n  http://myhost/rest/api/content/123/child/attachment/att456/data\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.updateAttachmentData_post
      x-api-path-slug: contentidchildattachmentattachmentiddata-post
      parameters:
      - in: path
        name: attachmentId
        description: The ID of the attachment to update
      - in: path
        name: id
        description: The ID of the content that the attachment is attached to
      responses:
        200:
          description: OK
      tags:
      - Attachment
      - Data
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