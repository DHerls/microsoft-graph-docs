---
title: "property resource type"
description: "A schema property definition for a Microsoft Search connection."
localization_priority: Normal
author: "snlraju-msft"
ms.prod: ""
doc_type: "resourcePageType"
---

# property resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A [schema](schema.md) property definition for a Microsoft Search [connection](connection.md).

## Properties

| Property      | Type    | Description                                        |
|:--------------|:--------|:---------------------------------------------------|
| isQueryable   | Boolean | Specifies if the property is queryable. Optional.  |
| isRetrievable | Boolean | Specifies if the property is retrievable. Optional. |
| isSearchable  | Boolean | Specifies if the property is searchable. Optional. |
| name          | String  | The name of the property. Required.                |
| type          | String  | The data type of the property. Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`. Required. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->