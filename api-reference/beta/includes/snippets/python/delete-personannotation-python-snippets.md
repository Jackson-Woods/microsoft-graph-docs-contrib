---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


await graph_client.users.by_user_id('user-id').profile.notes.by_person_annotation_id('personAnnotation-id').delete()


```