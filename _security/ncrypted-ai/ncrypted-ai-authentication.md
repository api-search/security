---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ncrypted Authentication
name_suffix: Authentication
oauth_flows: []
overview: ncrypted secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ncrypted
provider_slug: ncrypted-ai
scheme_count: 1
schemes:
- name: receiptToken
  scheme: bearer
  sources:
  - openapi/ncrypted-ai-openapi.json
  - openapi/ncrypted-ai-openapi.yml
  type: http
slug: ncrypted-ai-authentication
source_filename: ncrypted-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/ncrypted-ai-openapi.json, openapi/ncrypted-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: receiptToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ncrypted-ai-openapi.json\n  - openapi/ncrypted-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ncrypted-ai/authentication/ncrypted-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Secrets
- AI Agents
- Zero Knowledge
- Pay-per-use
---
