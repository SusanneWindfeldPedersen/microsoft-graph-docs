---
title: Create salesQuoteLines | Microsoft Docs
description: Creates a sales quote line object in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: "dynamics-365-business-central"
---

# Create salesQuoteLines
Create a sales quote line object in Dynamics 365 Business Central.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type |Permissions (from least to most privileged)|
|:---------------|:------------------------------------------|
|Delegated (work or school account)|Financials.ReadWrite.All |
|Delegated (personal Microsoft account|Not supported.|
|Application|Financials.ReadWrite.All|

## HTTP request

```
POST /financials/companies('{id}')/salesQuotes('{id}')/salesQuoteLines
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required.    |
|Content-Type  |application/json    |

## Request body
In the request body, supply a JSON representation of a **salesQuoteLines** object.

## Response
If successful, this method returns ```201 Created``` response code and a **salesQuoteLines** object in the response body.

## Example

**Request**

Here is an example of a request.

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/salesQuotes('{id}')/salesQuoteLines
Content-type: application/json

{
"itemId": "id-value",
"lineType": "Item",
"quantity": 9
}
```