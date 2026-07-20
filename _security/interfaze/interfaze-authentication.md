---
api_key_in: []
api_specs:
- filename: interfaze-openapi-original.json
  format: json
  label: Interfaze Chat Completion API
  slug: interfaze-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfaze/refs/heads/main/openapi/interfaze-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Interfaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interfaze secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Interfaze
provider_slug: interfaze
scheme_count: 1
schemes:
- description: API key obtained from the [dashboard](https://interfaze.ai/dashboard).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/interfaze-openapi-original.json
  type: http
slug: interfaze-authentication
source_filename: interfaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/interfaze-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from the [dashboard](https://interfaze.ai/dashboard).\n  sources:\n  - openapi/interfaze-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfaze/refs/heads/main/authentication/interfaze-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- OCR
- Speech to Text
- Structured Output
- Object Detection
- Web Scraping
- Web Search
- Multimodal
- Developer Tools
---
