---
title: "Get agedAccountsPayable"
description: "Retrieve the properties and relationships of agedaccountspayable object."
localization_priority: Normal
author: henrikwh
ms.prod: "dynamics-365-business-central"
doc_type: "apiPageType"
---

# Get agedAccountsPayable

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve the properties and relationships of an aged accounts payable report object for Dynamics 365 Business Central.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | Not supported. |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | Not supported. |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /financials/companies/{id}/agedAccountsPayable/{vendorId}
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

If successful, this method returns a `200 OK` response code and the requested [agedAccountsPayable](../resources/dynamics-agedaccountspayable.md) object in the response body.

## Examples

### Request

The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_agedaccountspayable"
}-->

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsPayable/{vendorId}
```

### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agedAccountsPayable"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "vendorId": "vendorId-value",
  "vendorNumber": "vendorNumber-value",
  "name": "name-value",
  "currencyCode": "currencyCode-value",
  "balanceDue": 99,
  "currentAmount": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get agedAccountsPayable",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->