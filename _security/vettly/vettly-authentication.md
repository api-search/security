---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vettly-content-moderation-openapi.json
  format: json
  label: Vettly REST API
  slug: vettly-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vettly/refs/heads/main/openapi/vettly-content-moderation-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vettly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vettly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vettly
provider_slug: vettly
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Enter your API key starting with vettly_live_ or vettly_test_
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vettly-content-moderation-openapi.json
  type: http
slug: vettly-authentication
source_filename: vettly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/vettly-content-moderation-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Enter your API key starting with vettly_live_ or vettly_test_\n  sources:\n  - openapi/vettly-content-moderation-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vettly/refs/heads/main/authentication/vettly-authentication.yml
summary_line: http · 1 scheme
tags:
- content-moderation
- trust-and-safety
- security
- text-analysis
- image-moderation
- video-moderation
- UGC
- compliance
- agent-guardrails
- MCP
---
