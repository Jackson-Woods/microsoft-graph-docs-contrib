---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = AccessPackageAssignmentRequest(
	request_type = "AdminRemove",
	access_package_assignment = AccessPackageAssignment(
		id = "a6bb6942-3ae1-4259-9908-0133aaee9377",
	),
)

result = await graph_client.identity_governance.entitlement_management.access_package_assignment_requests.post(request_body)


```