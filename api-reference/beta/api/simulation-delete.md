---
title: "Delete simulation"
description: "Delete an attack simulation campaign for a tenant."
author: stuartcl
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Delete simulation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete an attack simulation campaign for a tenant.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "simulation_delete" } -->
[!INCLUDE [permissions-table](../includes/permissions/simulation-delete-permissions.md)]

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /security/attackSimulation/simulations/{simulationId}
```

## Request headers

|Header         |Value                    |
|---------------|-------------------------|
|Authorization  |Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code in the response.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "delete_simulation",
  "sampleKeys": ["2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc"]
}
-->
```http
DELETE https://graph.microsoft.com/beta/security/attackSimulation/simulations/2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc
```

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
