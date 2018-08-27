---
name: Microsoft Office 365
x-slug: microsoft-office-365
description: Integrate Office 365 REST APIs powered by Microsoft Graph into your own
  app to connect to files, calendars, mail and more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Attachments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Office 365 - Get Contacts Contact Attachments
  x-api-slug: contactscontact-idattachments-get
  description: To get attachments, send a GET request to the Attachments pr...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-get-openapi.md
- name: Microsoft Office 365 - Add Contacts Contact Attachments
  x-api-slug: contactscontact-idattachments-post
  description: To add an attachment to an item, send a POST request to the ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-post-openapi.md
- name: Microsoft Office 365 - Delete Contacts Contact Attachments
  x-api-slug: contactscontact-idattachments-delete
  description: To delete an attachment, send a DELETE request to the URL of...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-delete-openapi.md
- name: Microsoft Office 365 - Parameters Contacts Contact Attachments
  x-api-slug: contactscontact-idattachments-parameters
  description: Parameters contacts contact  attachments
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/microsoft-office-365/contactscontact-idattachments-parameters-openapi.md
x-common:
- type: x-api-gallery
  url: http://microsoft.graph.api.gallery.streamdata.io
- type: x-api-stack
  url: http://microsoft.office.365.stack.network
- type: x-developer
  url: http://dev.office.com
- type: x-github
  url: https://github.com/OfficeDev
- type: x-twitter
  url: https://twitter.com/OfficeDev
- type: x-website
  url: http://office.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---