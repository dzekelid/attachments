{
  "info": {
    "name": "Kaltura VPaaS Get Service Attachment Attachmentasset Action Serve",
    "_postman_id": "c82bb385-f2ee-4dea-a621-b856f19f0916",
    "description": "Serves attachment by its id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "893e13a5-3b14-41f1-857c-fba0655ee724",
          "name": "attachmentAsset.add",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/add?attachmentAsset[accuracy]=%7B%7D&attachmentAsset[actualSourceAssetParamsIds]=%7B%7D&attachmentAsset[fileExt]=%7B%7D&attachmentAsset[filename]=%7B%7D&attachmentAsset[format]=%7B%7D&attachmentAsset[humanVerified]=%7B%7D&attachmentAsset[language]=%7B%7D&attachmentAsset[objectType]=%7B%7D&attachmentAsset[partnerData]=%7B%7D&attachmentAsset[partnerDescription]=%7B%7D&attachmentAsset[providerType]=%7B%7D&attachmentAsset[tags]=%7B%7D&attachmentAsset[title]=%7B%7D&entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment asset"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba59a2f1-ea44-4114-94cf-d1a5dc81f490"
            }
          ]
        },
        {
          "id": "40e10967-39b5-45c3-998a-b5e693103050",
          "name": "attachmentAsset.delete",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/delete?attachmentAssetId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Service Attachment Attachmentasset Action Delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "222b28f0-56fe-4849-9b00-85982ea72b9f"
            }
          ]
        },
        {
          "id": "abbe7d20-cfa1-415d-a0fc-652a8c21e6e8",
          "name": "attachmentAsset.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/get?attachmentAssetId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Service Attachment Attachmentasset Action Get"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7be23c79-4295-4949-b110-084d10a6b863"
            }
          ]
        },
        {
          "id": "8f8a7a7b-7d87-4041-aa1a-54dfe39dd116",
          "name": "attachmentAsset.getRemotePaths",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/getRemotePaths?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get remote storage existing paths for the asset"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c127f93c-4e4f-4faf-af5a-b5ee73a46f84"
            }
          ]
        },
        {
          "id": "e14fb98f-ce12-4703-8811-24ef1e2b1d75",
          "name": "attachmentAsset.getUrl",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/getUrl?id=%7B%7D&No Name=%7B%7D&storageId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get download URL for the asset"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e58e32eb-26a1-442e-a820-60fc75e4464a"
            }
          ]
        },
        {
          "id": "b4083341-e26d-4435-8546-8d675fc85de2",
          "name": "attachmentAsset.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/list?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[captionParamsIdEqual]=%7B%7D&filter[captionParamsIdIn]=%7B%7D&filter[contentLike]=%7B%7D&filter[contentMultiLikeAnd]=%7B%7D&filter[contentMultiLikeOr]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[deletedAtGreaterThanOrEqual]=%7B%7D&filter[deletedAtLessThanOrEqual]=%7B%7D&filter[endTimeGreaterThanOrEqual]=%7B%7D&filter[endTimeLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[entryIdIn]=%7B%7D&filter[flavorParamsIdEqual]=%7B%7D&filter[flavorParamsIdIn]=%7B%7D&filter[formatEqual]=%7B%7D&filter[formatIn]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[labelEqual]=%7B%7D&filter[labelIn]=%7B%7D&filter[languageEqual]=%7B%7D&filter[languageIn]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[partnerDescriptionLike]=%7B%7D&filter[partnerDescriptionMultiLikeAnd]=%7B%7D&filter[partnerDescriptionMultiLikeOr]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[sizeGreaterThanOrEqual]=%7B%7D&filter[sizeLessThanOrEqual]=%7B%7D&filter[startTimeGreaterThanOrEqual]=%7B%7D&filter[startTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[thumbParamsIdEqual]=%7B%7D&filter[thumbParamsIdIn]=%7B%7D&filter[typeIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List attachment Assets by filter and pager"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0281a671-d777-435f-8495-80b3185752df"
            }
          ]
        },
        {
          "id": "d07965d9-a651-461c-b779-f89d13860a05",
          "name": "attachmentAsset.serve",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/attachment_attachmentasset/action/serve?attachmentAssetId=%7B%7D&No Name=%7B%7D&serveOptions[download]=%7B%7D&serveOptions[referrer]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Serves attachment by its id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25cf7280-97b7-47cf-8f43-e38d3ab72f64"
            }
          ]
        }
      ]
    }
  ]
}