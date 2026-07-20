---
api_key_in:
- header
api_specs:
- filename: ask-sage-server-openapi.json
  format: json
  label: Ask Sage Server API
  slug: ask-sage-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/openapi/ask-sage-server-openapi.json
- filename: ask-sage-user-openapi.json
  format: json
  label: Ask Sage User API
  slug: ask-sage-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/openapi/ask-sage-user-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ask Sage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ask Sage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ask Sage
provider_slug: ask-sage
scheme_count: 1
schemes:
- description: JWT authentication token. Obtain a token by calling the User API endpoint `/user/get-token-with-api-key` with your email and API key.
  in: header
  name: ApiKeyAuth
  parameter: x-access-tokens
  sources:
  - openapi/ask-sage-server-openapi.json
  - openapi/ask-sage-user-openapi.json
  type: apiKey
slug: ask-sage-authentication
source_filename: ask-sage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/ask-sage-server-openapi.json, openapi/ask-sage-user-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-access-tokens\n  description: JWT authentication token. Obtain a token by calling the User API endpoint `/user/get-token-with-api-key`\n    with your email and API key.\n  sources:\n  - openapi/ask-sage-server-openapi.json\n  - openapi/ask-sage-user-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/authentication/ask-sage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Generative AI
- Large Language Models
- Government
- Defense
- Compliance
- FedRAMP
---
