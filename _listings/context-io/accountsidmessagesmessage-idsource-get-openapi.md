---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Messages Message Source
  description: 'Fetches the message source. Returns the raw RFC-822 message source
    for the message (including attachments) with no parsing or decoding to any portions
    of the message. On-demand data retrieval: since we do not keep full copies of
    emails on our servers, this call triggers a connection to the IMAP server to fetch
    the message. Attachments are part of the message source so they will impact how
    fast this call responds.'
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/messages/{message_id}/source:
    get:
      summary: Get Accounts Messages Message Source
      description: 'Fetches the message source. Returns the raw RFC-822 message source
        for the message (including attachments) with no parsing or decoding to any
        portions of the message. On-demand data retrieval: since we do not keep full
        copies of emails on our servers, this call triggers a connection to the IMAP
        server to fetch the message. Attachments are part of the message source so
        they will impact how fast this call responds.'
      operationId: getAccountMessageSource_
      x-api-path-slug: accountsidmessagesmessage-idsource-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Source
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