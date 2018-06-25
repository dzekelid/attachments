---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Attachments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: bitbucket
  description: |-
    Returns all attachments for this issue.

    This returns the files' meta data. This does not return the files'
    actual contents.

    The files are always ordered by their upload date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug issues issue  attachments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-parameters-openapi.md
- name: Bitbucket Add Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: bitbucket
  description: |-
    Upload new issue attachments.

    To upload files, perform a `multipart/form-data` POST containing one
    or more file fields.

    When a file is uploaded with the same name as an existing attachment,
    then the existing file will be replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-post-openapi.md
- name: Bitbucket Delete Repositories Username Repo Slug Issues Issue  Attachments
    Path
  x-api-slug: bitbucket
  description: Delete repositories username repo slug issues issue  attachments path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments/{path}
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments, Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Issues Issue  Attachments Path
  x-api-slug: bitbucket
  description: |-
    Returns the contents of the specified file attachment.

    Note that this endpoint does not return a JSON response, but instead
    returns a redirect pointing to the actual file that in turn will return
    the raw contents.

    The redirect URL contains a one-time token that has a limited lifetime.
    As a result, the link should not be persisted, stored, or shared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments/{path}
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments, Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Issues Issue  Attachments
    Path
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug issues issue  attachments
    path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/attachments/{path}
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Attachments, Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attachments/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---