---
title: "Get identityProtectionNotificationPolicy"
description: "Retrieve the properties and relationships of identityprotectionnotificationpolicy object."
localization_priority: Normal
author: "cloudhandler"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get identityProtectionNotificationPolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve the properties and relationships of identityprotectionnotificationpolicy object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | identityRiskyUser.Read.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | identityRiskyUser.Read.All |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /identityProtectionNotificationPolicy
```

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name      |Description|
|:----------|:----------|
| Authorization | Bearer {token} |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and the requested [identityProtectionNotificationPolicy](../resources/identityprotectionnotificationpolicy.md) object in the response body.

## Examples

### Request

The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_identityprotectionnotificationpolicy"
}-->

```http
GET https://graph.microsoft.com/BETA/identityProtectionNotificationPolicy
```

### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProtectionNotificationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "description": "description-value",
  "weeklyDigestSettings": {
    "isNotificationEnabled": true,
    "notificationRecipients": [
      "notificationRecipients-value"
    ],
    "additionalRecipients": [
      "additionalRecipients-value"
    ]
  },
  "userAlertsSettings": {
    "riskLevel": "riskLevel-value",
    "notificationRecipients": [
      "notificationRecipients-value"
    ],
    "additionalRecipients": [
      "additionalRecipients-value"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProtectionNotificationPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->