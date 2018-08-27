---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Attachment Attachmentasset Action Delete
  description: ""
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/attachment_attachmentasset/action/add:
    get:
      summary: Get Service Attachment Attachmentasset Action Add
      description: Add attachment asset
      operationId: attachmentAsset.add
      x-api-path-slug: serviceattachment-attachmentassetactionadd-get
      parameters:
      - in: query
        name: attachmentAsset[accuracy]
        description: The accuracy of the transcript - values between 0 and 1
      - in: query
        name: attachmentAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: attachmentAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: attachmentAsset[filename]
        description: The filename of the attachment asset content
      - in: query
        name: attachmentAsset[format]
        description: 'Enum Type: `KalturaAttachmentType`The attachment format'
      - in: query
        name: attachmentAsset[humanVerified]
        description: 'Enum Type: `KalturaNullableBoolean`Was verified by human or
          machine'
      - in: query
        name: attachmentAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the transcript'
      - in: query
        name: attachmentAsset[objectType]
      - in: query
        name: attachmentAsset[partnerData]
        description: Partner private data
      - in: query
        name: attachmentAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: attachmentAsset[providerType]
        description: 'Enum Type: `KalturaTranscriptProviderType`The provider of the
          transcript'
      - in: query
        name: attachmentAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: attachmentAsset[title]
        description: Attachment asset title
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Add
  /service/attachment_attachmentasset/action/delete:
    get:
      summary: Get Service Attachment Attachmentasset Action Delete
      description: ""
      operationId: attachmentAsset.delete
      x-api-path-slug: serviceattachment-attachmentassetactiondelete-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Delete
  /service/attachment_attachmentasset/action/get:
    get:
      summary: Get Service Attachment Attachmentasset Action Get
      description: ""
      operationId: attachmentAsset.get
      x-api-path-slug: serviceattachment-attachmentassetactionget-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Get
  /service/attachment_attachmentasset/action/getRemotePaths:
    get:
      summary: Get Service Attachment Attachmentasset Action Getremotepaths
      description: Get remote storage existing paths for the asset
      operationId: attachmentAsset.getRemotePaths
      x-api-path-slug: serviceattachment-attachmentassetactiongetremotepaths-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - GetRemotePaths
  /service/attachment_attachmentasset/action/getUrl:
    get:
      summary: Get Service Attachment Attachmentasset Action Geturl
      description: Get download URL for the asset
      operationId: attachmentAsset.getUrl
      x-api-path-slug: serviceattachment-attachmentassetactiongeturl-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: storageId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - GetUrl
  /service/attachment_attachmentasset/action/list:
    get:
      summary: Get Service Attachment Attachmentasset Action List
      description: List attachment Assets by filter and pager
      operationId: attachmentAsset.list
      x-api-path-slug: serviceattachment-attachmentassetactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[captionParamsIdEqual]
      - in: query
        name: filter[captionParamsIdIn]
      - in: query
        name: filter[contentLike]
      - in: query
        name: filter[contentMultiLikeAnd]
      - in: query
        name: filter[contentMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[deletedAtGreaterThanOrEqual]
      - in: query
        name: filter[deletedAtLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[flavorParamsIdEqual]
      - in: query
        name: filter[flavorParamsIdIn]
      - in: query
        name: filter[formatEqual]
        description: 'Enum Type: `KalturaAttachmentType`'
      - in: query
        name: filter[formatIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[labelEqual]
      - in: query
        name: filter[labelIn]
      - in: query
        name: filter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: filter[languageIn]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerDescriptionLike]
      - in: query
        name: filter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: filter[partnerDescriptionMultiLikeOr]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[sizeGreaterThanOrEqual]
      - in: query
        name: filter[sizeLessThanOrEqual]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaAttachmentAssetStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[thumbParamsIdEqual]
      - in: query
        name: filter[thumbParamsIdIn]
      - in: query
        name: filter[typeIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - List
  /service/attachment_attachmentasset/action/serve:
    get:
      summary: Get Service Attachment Attachmentasset Action Serve
      description: Serves attachment by its id
      operationId: attachmentAsset.serve
      x-api-path-slug: serviceattachment-attachmentassetactionserve-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      - in: query
        name: serveOptions[download]
      - in: query
        name: serveOptions[referrer]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Serve
  /service/attachment_attachmentasset/action/setContent:
    post:
      summary: Post Service Attachment Attachmentasset Action Setcontent
      description: Update content of attachment asset
      operationId: attachmentAsset.setContent
      x-api-path-slug: serviceattachment-attachmentassetactionsetcontent-post
      parameters:
      - in: query
        name: contentResource[assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[content]
        description: Textual content
      - in: query
        name: contentResource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[objectType]
      - in: query
        name: contentResource[privateKey]
        description: SSH private key
      - in: query
        name: contentResource[publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resources]
      - in: query
        name: contentResource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][objectType]
      - in: query
        name: contentResource[resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resources]
      - in: query
        name: contentResource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[token]
        description: Token that returned from upload
      - in: query
        name: contentResource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[version]
        description: The version of the file sync object
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - SetContent
  /service/attachment_attachmentasset/action/update:
    get:
      summary: Get Service Attachment Attachmentasset Action Update
      description: Update attachment asset
      operationId: attachmentAsset.update
      x-api-path-slug: serviceattachment-attachmentassetactionupdate-get
      parameters:
      - in: query
        name: attachmentAsset[accuracy]
        description: The accuracy of the transcript - values between 0 and 1
      - in: query
        name: attachmentAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: attachmentAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: attachmentAsset[filename]
        description: The filename of the attachment asset content
      - in: query
        name: attachmentAsset[format]
        description: 'Enum Type: `KalturaAttachmentType`The attachment format'
      - in: query
        name: attachmentAsset[humanVerified]
        description: 'Enum Type: `KalturaNullableBoolean`Was verified by human or
          machine'
      - in: query
        name: attachmentAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the transcript'
      - in: query
        name: attachmentAsset[objectType]
      - in: query
        name: attachmentAsset[partnerData]
        description: Partner private data
      - in: query
        name: attachmentAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: attachmentAsset[providerType]
        description: 'Enum Type: `KalturaTranscriptProviderType`The provider of the
          transcript'
      - in: query
        name: attachmentAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: attachmentAsset[title]
        description: Attachment asset title
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Update
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