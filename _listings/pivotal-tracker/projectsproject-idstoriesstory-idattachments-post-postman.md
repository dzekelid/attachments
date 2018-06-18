{
  "info": {
    "name": "Pivotal Tracker Post Projects Project Stories Story Attachments",
    "_postman_id": "79b95763-32bc-4180-a535-2bc65c76bd38",
    "description": "Post projects project stories story attachments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "d6715350-0885-47ae-8937-5931f68d6b3b",
          "name": "postProjectsProjectStoriesStoryAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/attachments"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post projects project stories story attachments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fcd0c15-f035-43b7-86df-3c248086d64c"
            }
          ]
        }
      ]
    }
  ]
}