{
  "info": {
    "name": "Microsoft Office 365 Get Contacts Contact Attachments",
    "_postman_id": "514be1a5-97d8-461f-8755-6bf04a6af131",
    "description": "To get attachments, send a GET request to the Attachments pr...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "contacts",
      "item": [
        {
          "id": "16ef075e-7025-4d74-af17-cb6d7827886d",
          "name": "getContactsContactAttachments",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To get attachments, send a GET request to the Attachments pr"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0400d2a-570d-42bb-9137-8e1c6b60a4bb"
            }
          ]
        }
      ]
    }
  ]
}