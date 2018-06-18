---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Invoices Invoice Attachments
  description: Get invoices invoice attachments.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountID}/Attachments:
    get:
      summary: Get Accounts Attachments
      description: Get accounts account attachments.
      operationId: getAccountsAccountAttachments
      x-api-path-slug: accountsaccountidattachments-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
  /Accounts/{AccountID}/Attachments/{FileName}:
    get:
      summary: Get Accounts Attachments Filename
      description: Get accounts account attachments filename.
      operationId: getAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
    post:
      summary: Post Accounts Attachments Filename
      description: Post accounts account attachments filename.
      operationId: postAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-post
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
  /BankTransactions/{BankTransactionID}/Attachments:
    get:
      summary: Get Bank Transactions Banktransaction Attachments
      description: Get banktransactions banktransaction attachments.
      operationId: getBanktransactionsBanktransactionAttachments
      x-api-path-slug: banktransactionsbanktransactionidattachments-get
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
  /BankTransactions/{BankTransactionID}/Attachments/{FileName}:
    get:
      summary: Get Bank Transactions Banktransaction Attachments Filename
      description: Get banktransactions banktransaction attachments filename.
      operationId: getBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
    post:
      summary: Post Bank Transactions Banktransaction Attachments Filename
      description: Post banktransactions banktransaction attachments filename.
      operationId: postBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
  /BankTransfers/{BankTransferID}/Attachments/{FileName}:
    get:
      summary: Get Banks Transfers Attachments Filename
      description: Get banktransfers banktransfer attachments filename.
      operationId: getBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for an BankTransfer
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
    post:
      summary: Post Banks Transfers Attachments Filename
      description: Post banktransfers banktransfer attachments filename.
      operationId: postBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for a BankTransfer
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
  /Contacts/{ContactID}/Attachments:
    get:
      summary: Get Contacts Contact Attachments
      description: Get contacts contact attachments.
      operationId: getContactsContactAttachments
      x-api-path-slug: contactscontactidattachments-get
      parameters:
      - in: path
        name: ContactID
        description: The Xero generated unique identifier for a Contact
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - ContactID
      - Attachments
  /Contacts/{ContactID}/Attachments/{FileName}:
    get:
      summary: Get Contacts Contact Attachments Filename
      description: Get contacts contact attachments filename.
      operationId: getContactsContactAttachmentsFilename
      x-api-path-slug: contactscontactidattachmentsfilename-get
      parameters:
      - in: path
        name: ContactID
        description: The Xero generated unique identifier for a Contact
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - ContactID
      - Attachments
      - FileName
    post:
      summary: Post Contacts Contact Attachments Filename
      description: Post contacts contact attachments filename.
      operationId: postContactsContactAttachmentsFilename
      x-api-path-slug: contactscontactidattachmentsfilename-post
      parameters:
      - in: path
        name: ContactID
        description: The Xero generated unique identifier for a Contact
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - ContactID
      - Attachments
      - FileName
  /CreditNotes/{CreditNoteID}/Attachments:
    get:
      summary: Get Creditnotes Creditnote Attachments
      description: Get creditnotes creditnote attachments.
      operationId: getCreditnotesCreditnoteAttachments
      x-api-path-slug: creditnotescreditnoteidattachments-get
      parameters:
      - in: path
        name: CreditNoteID
        description: The Xero generated unique identifier for a CreditNote
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - CreditNotes
      - CreditNoteID
      - Attachments
  /CreditNotes/{CreditNoteID}/Attachments/{FileName}:
    get:
      summary: Get Creditnotes Creditnote Attachments Filename
      description: Get creditnotes creditnote attachments filename.
      operationId: getCreditnotesCreditnoteAttachmentsFilename
      x-api-path-slug: creditnotescreditnoteidattachmentsfilename-get
      parameters:
      - in: path
        name: CreditNoteID
        description: The Xero generated unique identifier for a CreditNote
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - CreditNotes
      - CreditNoteID
      - Attachments
      - FileName
    post:
      summary: Post Creditnotes Creditnote Attachments Filename
      description: Post creditnotes creditnote attachments filename.
      operationId: postCreditnotesCreditnoteAttachmentsFilename
      x-api-path-slug: creditnotescreditnoteidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: CreditNoteID
        description: The Xero generated unique identifier for a CreditNote
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - CreditNotes
      - CreditNoteID
      - Attachments
      - FileName
  /Invoices/{InvoiceID}/Attachments:
    get:
      summary: Get Invoices Invoice Attachments
      description: Get invoices invoice attachments.
      operationId: getInvoicesInvoiceAttachments
      x-api-path-slug: invoicesinvoiceidattachments-get
      parameters:
      - in: path
        name: InvoiceID
        description: The Xero generated unique identifier for an Invoice
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Invoices
      - InvoiceID
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