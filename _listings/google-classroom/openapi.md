---
swagger: "2.0"
x-collection-name: Google Classroom
x-complete: 1
info:
  title: Google Classroom
  description: manages-classes-rosters-and-invitations-in-google-classroom-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: classroom.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:modifyAttachments:
    post:
      summary: Modify Attachments
      description: |-
        Modifies attachments of student submission.

        Attachments may only be added to student submissions belonging to course
        work objects with a `workType` of `ASSIGNMENT`.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, if the user is not permitted to modify
        attachments on the requested student submission, or for
        access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.modifyAttachments
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsidmodifyattachments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Attachment
---