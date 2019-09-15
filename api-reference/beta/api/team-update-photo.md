---
title: "Update team photo"
description: "Update the photo (picture) for a team."
author: "clearab"
localization_priority: Priority
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# Update team photo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the photo (picture) for a team. The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648. Photos can be any dimension if they are stored in Azure Active Directory.

> Note: There is a limit of 4 MB on the total size of the request. This limits the photo size to less than 4 MB.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Group.ReadWrite.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Group.ReadWrite.All |

## HTTP Request

<!-- {
  "blockType": "request",
  "name": "update_team_photo"
}-->

```http
PUT /beta/teams/{id}/photo
content-type: image/jpeg

Binary data for the image
```

## Request headers

| Header        | Value           |
|:--------------|:--------------  |
| Authorization | Bearer {token}. Required.  |
| Content-type | image/jpeg. Required.  |

## Request body

In the request body, include the binary data of the photo.

## Response

If successful, this method returns a `200 OK` response code

## Example

### Request

Here is an example of the request.

<!-- {
  "blockType": "request",
  "name": "update_team_photo"
}-->
```http
https://graph.microsoft.com/beta/teams/{id}/photo
```

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->