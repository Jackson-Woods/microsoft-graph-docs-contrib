---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = RegionalAndLanguageSettings(
	authoring_languages = [
		LocaleInfo(
			locale = "en-US",
		),
		LocaleInfo(
			locale = "es-MX",
		),
	],
	default_regional_format = LocaleInfo(
		locale = "en-US",
	),
)

result = await graph_client.me.settings.regional_and_language_settings.patch(request_body)


```