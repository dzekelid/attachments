swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{PROJECT_ID}/stories/{STORY_ID}/attachments:
    post:
      summary: Post Projects Project Stories Story Attachments
      description: Post projects project stories story attachments.
      operationId: postProjectsProjectStoriesStoryAttachments
      x-api-path-slug: projectsproject-idstoriesstory-idattachments-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Attachments