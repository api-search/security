---
anonymous_access: false
api_key_in:
- cookie
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: docbin Authentication
name_suffix: Authentication
oauth_flows: []
overview: docbin secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: docbin
provider_slug: docbin-app
scheme_count: 2
schemes:
- description: API key as `dbk_...`
  name: Bearer
  scheme: bearer
  sources:
  - openapi/docbin-app-openapi.json
  type: http
- description: Browser session cookie. An API key cannot manage API keys.
  in: cookie
  name: Session
  parameter: db_session
  sources:
  - openapi/docbin-app-openapi.json
  type: apiKey
slug: docbin-app-authentication
source_filename: docbin-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/docbin-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: API key as `dbk_...`\n  sources:\n  - openapi/docbin-app-openapi.json\n- name: Session\n  type: apiKey\n  in: cookie\n  parameter: db_session\n  description: Browser session cookie. An API key cannot manage API keys.\n  sources:\n  - openapi/docbin-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/docbin-app/authentication/docbin-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Pastebin
- Markdown
- CLI
- Documentation
---
