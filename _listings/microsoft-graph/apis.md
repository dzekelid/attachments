---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Attachments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
  tags: List, Attachments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/memailfoldersidchildfoldersid---messagesidattachmentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/memailfoldersidchildfoldersid---messagesidattachmentsid-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
  tags: List, Attachments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidchildfoldersidmessagesidattachmentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidchildfoldersidmessagesidattachmentsid-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/meeventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnameeventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/groupsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendar/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/mecalendareventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendar/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamecalendareventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/calendar/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/groupsidcalendareventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/mecalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamecalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendargroup/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/mecalendargroupcalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupcalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/mecalendargroupsidcalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    an event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupsidcalendarsideventsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/messages/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/memessagesidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/messages/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamemessagesidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}/messages/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/memailfoldersidmessagesidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidmessagesidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a post.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/threads/{id}/posts/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/groupsidthreadsidpostsidattachments-get-openapi.md
- name: Microsoft Graph List Attachments
  x-api-slug: microsoft-graph
  description: List attachments Retrieve a list of attachment objects attached to
    a post.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
  tags: List, Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/groupsidconversationsidthreadsidpostsidattachments-get-openapi.md
- name: Microsoft Graph
  x-api-slug: microsoft-graph
  description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
    cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
    Graph simplifies queries that would otherwise be more complex. You can use Microsoft
    Graph to: Access data from multiple Microsoft cloud services, including Azure
    Active Directory, Exchange Online as part of Office 365, SharePoint, OneDrive,
    OneNote, and Planner. Navigate between entities and relationships. Access intelligence
    and insights from the Microsoft cloud (for commercial users).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-graph/openapi.md
x-common:
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---