{
  "info": {
    "name": "Microsoft Office 365 Delete Contacts Contact Attachments",
    "_postman_id": "b2692a38-2b4d-4b89-8b1b-f2d8b5069ec9",
    "description": "To delete an attachment, send a DELETE request to the URL of...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "contacts",
      "item": [
        {
          "id": "ef6ce49e-85a8-4142-a19e-989cfa41cab6",
          "name": "deleteContactsContactAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "Contacts:contact_id/Attachments"
              ],
              "variable": [
                {
                  "id": "contact_id",
                  "value": "contact_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "To delete an attachment, send a DELETE request to the URL of"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17c39e1c-52ab-448d-bf59-281c25bcac7b"
            }
          ]
        }
      ]
    }
  ]
}