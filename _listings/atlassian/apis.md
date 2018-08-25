---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Attachments
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Get attachments
  x-api-slug: contentidchildattachment-get
  description: "Returns the attachments for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to view the content. If the content is a blog post, 'View'
    permission \nfor the space is required."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-get-openapi.md
- name: The Confluence Cloud REST API - Create attachment
  x-api-slug: contentidchildattachment-post
  description: "Adds an attachment to a piece of content. This method only adds a
    new \nattachment. If you want to update an existing attachment, use \n[Create
    or update attachments](#api-content-id-child-attachment-put).\n\nNote, you must
    set a `X-Atlassian-Token: nocheck` header on the request \nfor this method, otherwise
    it will be blocked. This protects against XSRF \nattacks, which is necessary as
    this method accepts multipart/form-data.\n\nThe media type 'multipart/form-data'
    is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client
    libraries have classes that make it easier to implement \nmultipart posts, like
    the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    attaches a file ('example.txt') to a container \n(id='123') with a comment and
    `minorEdits`=true.\n\n``` bash\ncurl -D- \\\n  -u admin:admin \\\n  -X POST \\\n
    \ -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\" \\\n  -F \"minorEdit=true\"
    \\\n  -F \"comment=Example attachment comment\" \\\n  http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-post-openapi.md
- name: The Confluence Cloud REST API - Create or update attachment
  x-api-slug: contentidchildattachment-put
  description: "Adds an attachment to a piece of content. If the attachment already
    exists \nfor the content, then the attachment is updated (i.e. a new version of
    the \nattachment is created).\n\nNote, you must set a `X-Atlassian-Token: nocheck`
    header on the request \nfor this method, otherwise it will be blocked. This protects
    against XSRF \nattacks, which is necessary as this method accepts multipart/form-data.\n\nThe
    media type 'multipart/form-data' is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt).
    \nMost client libraries have classes that make it easier to implement \nmultipart
    posts, like the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    attaches a file ('example.txt') to a piece of \ncontent (id='123') with a comment
    and `minorEdits`=true. If the 'example.txt' \nfile already exists, it will update
    it with a new version of the attachment.\n\n``` bash\ncurl -D- \\\n  -u admin:admin
    \\\n  -X PUT \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
    \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\" \\\n
    \ http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-put-openapi.md
- name: The Confluence Cloud REST API - Update attachment properties
  x-api-slug: contentidchildattachmentattachmentid-put
  description: "Updates the attachment properties, i.e. the non-binary data of an
    attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentid-put-openapi.md
- name: The Confluence Cloud REST API - Update attachment data
  x-api-slug: contentidchildattachmentattachmentiddata-post
  description: "Updates the binary data of an attachment, given the attachment ID,
    and \noptionally the comment and the minor edit field.\n\nThis method is essentially
    the same as [Create or update attachments](#api-content-id-child-attachment-put),
    \nexcept that it matches the attachment ID rather than the name.\n\nNote, you
    must set a `X-Atlassian-Token: nocheck` header on the request \nfor this method,
    otherwise it will be blocked. This protects against XSRF \nattacks, which is necessary
    as this method accepts multipart/form-data.\n\nThe media type 'multipart/form-data'
    is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client
    libraries have classes that make it easier to implement \nmultipart posts, like
    the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    updates an attachment (id='att456') that is attached  \nto a piece of content
    (id='123') with a comment and `minorEdits`=true. \n\n``` bash\ncurl -D- \\\n  -u
    admin:admin \\\n  -X POST \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
    \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\" \\\n
    \ http://myhost/rest/api/content/123/child/attachment/att456/data\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentiddata-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentiddata-post-openapi.md
- name: The Confluence Cloud REST API - Create attachment
  x-api-slug: contentidchildattachment-post
  description: "Adds an attachment to a piece of content. This method only adds a
    new \nattachment. If you want to update an existing attachment, use \n[Create
    or update attachments](#api-content-id-child-attachment-put).\n\nNote, you must
    set a `X-Atlassian-Token: nocheck` header on the request \nfor this method, otherwise
    it will be blocked. This protects against XSRF \nattacks, which is necessary as
    this method accepts multipart/form-data.\n\nThe media type 'multipart/form-data'
    is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client
    libraries have classes that make it easier to implement \nmultipart posts, like
    the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    attaches a file ('example.txt') to a container \n(id='123') with a comment and
    `minorEdits`=true.\n\n``` bash\ncurl -D- \\\n  -u admin:admin \\\n  -X POST \\\n
    \ -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\" \\\n  -F \"minorEdit=true\"
    \\\n  -F \"comment=Example attachment comment\" \\\n  http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-post-openapi.md
- name: The Confluence Cloud REST API - Create or update attachment
  x-api-slug: contentidchildattachment-put
  description: "Adds an attachment to a piece of content. If the attachment already
    exists \nfor the content, then the attachment is updated (i.e. a new version of
    the \nattachment is created).\n\nNote, you must set a `X-Atlassian-Token: nocheck`
    header on the request \nfor this method, otherwise it will be blocked. This protects
    against XSRF \nattacks, which is necessary as this method accepts multipart/form-data.\n\nThe
    media type 'multipart/form-data' is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt).
    \nMost client libraries have classes that make it easier to implement \nmultipart
    posts, like the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    attaches a file ('example.txt') to a piece of \ncontent (id='123') with a comment
    and `minorEdits`=true. If the 'example.txt' \nfile already exists, it will update
    it with a new version of the attachment.\n\n``` bash\ncurl -D- \\\n  -u admin:admin
    \\\n  -X PUT \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
    \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\" \\\n
    \ http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachment-put-openapi.md
- name: The Confluence Cloud REST API - Update attachment properties
  x-api-slug: contentidchildattachmentattachmentid-put
  description: "Updates the attachment properties, i.e. the non-binary data of an
    attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentid-put-openapi.md
- name: The Confluence Cloud REST API - Update attachment data
  x-api-slug: contentidchildattachmentattachmentiddata-post
  description: "Updates the binary data of an attachment, given the attachment ID,
    and \noptionally the comment and the minor edit field.\n\nThis method is essentially
    the same as [Create or update attachments](#api-content-id-child-attachment-put),
    \nexcept that it matches the attachment ID rather than the name.\n\nNote, you
    must set a `X-Atlassian-Token: nocheck` header on the request \nfor this method,
    otherwise it will be blocked. This protects against XSRF \nattacks, which is necessary
    as this method accepts multipart/form-data.\n\nThe media type 'multipart/form-data'
    is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client
    libraries have classes that make it easier to implement \nmultipart posts, like
    the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    updates an attachment (id='att456') that is attached  \nto a piece of content
    (id='123') with a comment and `minorEdits`=true. \n\n``` bash\ncurl -D- \\\n  -u
    admin:admin \\\n  -X POST \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
    \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\" \\\n
    \ http://myhost/rest/api/content/123/child/attachment/att456/data\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentiddata-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/contentidchildattachmentattachmentiddata-post-openapi.md
- name: Jira Cloud REST API - Get global attachment settings
  x-api-slug: api2attachmentmeta-get
  description: "Returns the global attachment settings, that is, whether attachments
    are enabled and the maximum attachment size allowed.  \n  \nNote that there are
    also [project permissions](https://confluence.atlassian.com/x/yodKLg) that restrict
    whether users can create and delete attachments or not.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentmeta-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentmeta-get-openapi.md
- name: Jira Cloud REST API - Get attachment metadata
  x-api-slug: api2attachmentid-get
  description: "Returns the metadata for an attachment. Note that the attachment itself
    is not returned.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-get-openapi.md
- name: Jira Cloud REST API - Delete attachment
  x-api-slug: api2attachmentid-delete
  description: "Deletes an attachment from an issue.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Any of the following permissions in the project that the issue is
    in:\n\n*   _Delete own attachments_ [project permission](https://confluence.atlassian.com/x/yodKLg)
    to delete an attachment created by the calling user.\n*   _Delete all attachments_
    [project permission](https://confluence.atlassian.com/x/yodKLg) to delete an attachment
    created by any user."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-delete-openapi.md
- name: Jira Cloud REST API - Get all metadata for an expanded attachment
  x-api-slug: api2attachmentidexpandhuman-get
  description: "Returns the metadata for the contents of an attachment, if it is an
    archive, and metadata for the attachment itself. For example, if the attachment
    is a ZIP archive, then information about the files in the archive is returned
    and metadata for the ZIP archive. Currently, only the ZIP archive format is supported.
    \ \n  \nUse this method to retrieve data that is presented in the UI, as this
    method returns the metadata for the attachment itself, such as the attachment's
    ID and name. Otherwise, use [Get contents metadata for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-raw-get),
    which only returns the metadata for the attachment's contents.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandhuman-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandhuman-get-openapi.md
- name: Jira Cloud REST API - Get contents metadata for an expanded attachment
  x-api-slug: api2attachmentidexpandraw-get
  description: "Returns the metadata for the contents of an attachment, if it is an
    archive. For example, if the attachment is a ZIP archive, then information about
    the files in the archive is returned. Currently, only the ZIP archive format is
    supported.  \n  \nUse this method if you are processing the data without presenting
    it in the UI, as this method only returns the metadata for the contents of the
    attachment. Otherwise, to retrieve data to present in the UI, use [Get all metadata
    for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-human-get)
    which also returns the metadata for the attachment itself, such as the attachment's
    ID and name.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandraw-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandraw-get-openapi.md
- name: Jira Cloud REST API - Add attachment
  x-api-slug: api2issueissueidorkeyattachments-post
  description: |-
    Add one or more attachments to an issue.

    This resource expects a multipart post. The media-type multipart/form-data is defined in RFC 1867. Most client libraries have classes that make dealing with multipart posts simple. For instance, in Java the Apache HTTP Components library provides a [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html) that makes it simple to submit a multipart POST.

    In order to protect against XSRF attacks, because this method accepts multipart/form-data, it has XSRF protection on it. This means you must submit a header of X-Atlassian-Token: no-check with the request, otherwise it will be blocked.

    The name of the multipart/form-data parameter that contains attachments must be "file"

    A simple example to upload a file called "myfile.txt" to issue REST-123:

    curl -D- -u admin:admin -X POST -H "X-Atlassian-Token: no-check" -F "file=@myfile.txt" http://myhost/rest/api/2/issue/TEST-123/attachments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2issueissueidorkeyattachments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2issueissueidorkeyattachments-post-openapi.md
- name: Jira Cloud REST API - Get all permission schemes
  x-api-slug: api2permissionscheme-get
  description: |-
    Returns all permission schemes.

    ### About permission schemes and grants

    A permission scheme is a collection of permission grants. A permission grant consists of a `holder` and a `permission`.

    #### Holder

    The `holder` object contains information about the user or group being granted the permission. For example, the _Administer projects_ permission is granted to a group named _Teams in space administrators_. In this case, the type is `"type": "group"`, and the parameter is the group name, `"parameter": "Teams in space administrators"`. The `holder` object is defined by the following properties:

    *   `type` Identifies the user or group (see the list of types below).
    *   `parameter` The value of this property depends on the `type`. For example, if the `type` is a group, then you need to specify the group name.

    The following `types` are available. The expected values for the `parameter` are given in parenthesis (some `types` may not have a `parameter`):

    *   `anyone` Grant for anonymous users.
    *   `applicationRole` Grant for users with access to the specified application (application name). See [Manage application access](https://confluence.atlassian.com/cloud/manage-application-access-744721629.html) for more information.
    *   `assignee` Grant for the user currently assigned to an issue.
    *   `group` Grant for the specified group (group name).
    *   `groupCustomField` Grant for a user in the group selected in the specified custom field (custom field ID).
    *   `projectLead` Grant for a project lead.
    *   `projectRole` Grant for the specified project role (project role ID).
    *   `reporter` Grant for the user who reported the issue.
    *   `sd.customer.portal.only` Jira Service Desk only. Grants customers permission to access the customer portal but not Jira. See [Customizing Jira Service Desk permissions](https://confluence.atlassian.com/x/24dKLg) for more information.
    *   `user` Grant for the specified user (user ID).
    *   `userCustomField` Grant for a user selected in the specified custom field (custom field ID).

    #### Permissions

    The [built-in Jira permissions](https://confluence.atlassian.com/x/yodKLg) are listed below. Apps can also define custom permissions. See the [project permission](https://developer.atlassian.com/cloud/jira/platform/modules/project-permission/) and [global permission](https://developer.atlassian.com/cloud/jira/platform/modules/global-permission/) module documentation for more information.

    **Project permissions**

    *   `ADMINISTER_PROJECTS`
    *   `BROWSE_PROJECTS`
    *   `MANAGE_SPRINTS_PERMISSION` (Jira Software only)
    *   `SERVICEDESK_AGENT` (Jira Service Desk only)
    *   `VIEW_DEV_TOOLS` (Jira Software only)
    *   `VIEW_READONLY_WORKFLOW`

    **Issue permissions**

    *   `ASSIGNABLE_USER`
    *   `ASSIGN_ISSUES`
    *   `CLOSE_ISSUES`
    *   `CREATE_ISSUES`
    *   `DELETE_ISSUES`
    *   `EDIT_ISSUES`
    *   `LINK_ISSUES`
    *   `MODIFY_REPORTER`
    *   `MOVE_ISSUES`
    *   `RESOLVE_ISSUES`
    *   `SCHEDULE_ISSUES`
    *   `SET_ISSUE_SECURITY`
    *   `TRANSITION_ISSUES`

    **Voters and watchers permissions**

    *   `MANAGE_WATCHERS`
    *   `VIEW_VOTERS_AND_WATCHERS`

    **Comments permissions**

    *   `ADD_COMMENTS`
    *   `DELETE_ALL_COMMENTS`
    *   `DELETE_OWN_COMMENTS`
    *   `EDIT_ALL_COMMENTS`
    *   `EDIT_OWN_COMMENTS`

    **Attachments permissions**

    *   `CREATE_ATTACHMENTS`
    *   `DELETE_ALL_ATTACHMENTS`
    *   `DELETE_OWN_ATTACHMENTS`

    **Time tracking permissions**

    *   `DELETE_ALL_WORKLOGS`
    *   `DELETE_OWN_WORKLOGS`
    *   `EDIT_ALL_WORKLOGS`
    *   `EDIT_OWN_WORKLOGS`
    *   `WORK_ON_ISSUES`

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2permissionscheme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2permissionscheme-get-openapi.md
- name: Jira Cloud REST API - Get global attachment settings
  x-api-slug: api2attachmentmeta-get
  description: "Returns the global attachment settings, that is, whether attachments
    are enabled and the maximum attachment size allowed.  \n  \nNote that there are
    also [project permissions](https://confluence.atlassian.com/x/yodKLg) that restrict
    whether users can create and delete attachments or not.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentmeta-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentmeta-get-openapi.md
- name: Jira Cloud REST API - Get attachment metadata
  x-api-slug: api2attachmentid-get
  description: "Returns the metadata for an attachment. Note that the attachment itself
    is not returned.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-get-openapi.md
- name: Jira Cloud REST API - Delete attachment
  x-api-slug: api2attachmentid-delete
  description: "Deletes an attachment from an issue.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Any of the following permissions in the project that the issue is
    in:\n\n*   _Delete own attachments_ [project permission](https://confluence.atlassian.com/x/yodKLg)
    to delete an attachment created by the calling user.\n*   _Delete all attachments_
    [project permission](https://confluence.atlassian.com/x/yodKLg) to delete an attachment
    created by any user."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentid-delete-openapi.md
- name: Jira Cloud REST API - Get all metadata for an expanded attachment
  x-api-slug: api2attachmentidexpandhuman-get
  description: "Returns the metadata for the contents of an attachment, if it is an
    archive, and metadata for the attachment itself. For example, if the attachment
    is a ZIP archive, then information about the files in the archive is returned
    and metadata for the ZIP archive. Currently, only the ZIP archive format is supported.
    \ \n  \nUse this method to retrieve data that is presented in the UI, as this
    method returns the metadata for the attachment itself, such as the attachment's
    ID and name. Otherwise, use [Get contents metadata for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-raw-get),
    which only returns the metadata for the attachment's contents.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandhuman-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandhuman-get-openapi.md
- name: Jira Cloud REST API - Get contents metadata for an expanded attachment
  x-api-slug: api2attachmentidexpandraw-get
  description: "Returns the metadata for the contents of an attachment, if it is an
    archive. For example, if the attachment is a ZIP archive, then information about
    the files in the archive is returned. Currently, only the ZIP archive format is
    supported.  \n  \nUse this method if you are processing the data without presenting
    it in the UI, as this method only returns the metadata for the contents of the
    attachment. Otherwise, to retrieve data to present in the UI, use [Get all metadata
    for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-human-get)
    which also returns the metadata for the attachment itself, such as the attachment's
    ID and name.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** None, however the calling user must have permission to view the issue
    that the attachment belongs to."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandraw-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2attachmentidexpandraw-get-openapi.md
- name: Jira Cloud REST API - Add attachment
  x-api-slug: api2issueissueidorkeyattachments-post
  description: |-
    Add one or more attachments to an issue.

    This resource expects a multipart post. The media-type multipart/form-data is defined in RFC 1867. Most client libraries have classes that make dealing with multipart posts simple. For instance, in Java the Apache HTTP Components library provides a [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html) that makes it simple to submit a multipart POST.

    In order to protect against XSRF attacks, because this method accepts multipart/form-data, it has XSRF protection on it. This means you must submit a header of X-Atlassian-Token: no-check with the request, otherwise it will be blocked.

    The name of the multipart/form-data parameter that contains attachments must be "file"

    A simple example to upload a file called "myfile.txt" to issue REST-123:

    curl -D- -u admin:admin -X POST -H "X-Atlassian-Token: no-check" -F "file=@myfile.txt" http://myhost/rest/api/2/issue/TEST-123/attachments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2issueissueidorkeyattachments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2issueissueidorkeyattachments-post-openapi.md
- name: Jira Cloud REST API - Get all permission schemes
  x-api-slug: api2permissionscheme-get
  description: |-
    Returns all permission schemes.

    ### About permission schemes and grants

    A permission scheme is a collection of permission grants. A permission grant consists of a `holder` and a `permission`.

    #### Holder

    The `holder` object contains information about the user or group being granted the permission. For example, the _Administer projects_ permission is granted to a group named _Teams in space administrators_. In this case, the type is `"type": "group"`, and the parameter is the group name, `"parameter": "Teams in space administrators"`. The `holder` object is defined by the following properties:

    *   `type` Identifies the user or group (see the list of types below).
    *   `parameter` The value of this property depends on the `type`. For example, if the `type` is a group, then you need to specify the group name.

    The following `types` are available. The expected values for the `parameter` are given in parenthesis (some `types` may not have a `parameter`):

    *   `anyone` Grant for anonymous users.
    *   `applicationRole` Grant for users with access to the specified application (application name). See [Manage application access](https://confluence.atlassian.com/cloud/manage-application-access-744721629.html) for more information.
    *   `assignee` Grant for the user currently assigned to an issue.
    *   `group` Grant for the specified group (group name).
    *   `groupCustomField` Grant for a user in the group selected in the specified custom field (custom field ID).
    *   `projectLead` Grant for a project lead.
    *   `projectRole` Grant for the specified project role (project role ID).
    *   `reporter` Grant for the user who reported the issue.
    *   `sd.customer.portal.only` Jira Service Desk only. Grants customers permission to access the customer portal but not Jira. See [Customizing Jira Service Desk permissions](https://confluence.atlassian.com/x/24dKLg) for more information.
    *   `user` Grant for the specified user (user ID).
    *   `userCustomField` Grant for a user selected in the specified custom field (custom field ID).

    #### Permissions

    The [built-in Jira permissions](https://confluence.atlassian.com/x/yodKLg) are listed below. Apps can also define custom permissions. See the [project permission](https://developer.atlassian.com/cloud/jira/platform/modules/project-permission/) and [global permission](https://developer.atlassian.com/cloud/jira/platform/modules/global-permission/) module documentation for more information.

    **Project permissions**

    *   `ADMINISTER_PROJECTS`
    *   `BROWSE_PROJECTS`
    *   `MANAGE_SPRINTS_PERMISSION` (Jira Software only)
    *   `SERVICEDESK_AGENT` (Jira Service Desk only)
    *   `VIEW_DEV_TOOLS` (Jira Software only)
    *   `VIEW_READONLY_WORKFLOW`

    **Issue permissions**

    *   `ASSIGNABLE_USER`
    *   `ASSIGN_ISSUES`
    *   `CLOSE_ISSUES`
    *   `CREATE_ISSUES`
    *   `DELETE_ISSUES`
    *   `EDIT_ISSUES`
    *   `LINK_ISSUES`
    *   `MODIFY_REPORTER`
    *   `MOVE_ISSUES`
    *   `RESOLVE_ISSUES`
    *   `SCHEDULE_ISSUES`
    *   `SET_ISSUE_SECURITY`
    *   `TRANSITION_ISSUES`

    **Voters and watchers permissions**

    *   `MANAGE_WATCHERS`
    *   `VIEW_VOTERS_AND_WATCHERS`

    **Comments permissions**

    *   `ADD_COMMENTS`
    *   `DELETE_ALL_COMMENTS`
    *   `DELETE_OWN_COMMENTS`
    *   `EDIT_ALL_COMMENTS`
    *   `EDIT_OWN_COMMENTS`

    **Attachments permissions**

    *   `CREATE_ATTACHMENTS`
    *   `DELETE_ALL_ATTACHMENTS`
    *   `DELETE_OWN_ATTACHMENTS`

    **Time tracking permissions**

    *   `DELETE_ALL_WORKLOGS`
    *   `DELETE_OWN_WORKLOGS`
    *   `EDIT_ALL_WORKLOGS`
    *   `EDIT_OWN_WORKLOGS`
    *   `WORK_ON_ISSUES`

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2permissionscheme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/atlassian/api2permissionscheme-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---