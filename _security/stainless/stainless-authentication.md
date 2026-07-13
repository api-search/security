---
api_key_in: []
api_specs:
- filename: stainless-openapi.yml
  format: yaml
  label: Stainless SDK Generator
  slug: stainless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stainless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stainless secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stainless
provider_slug: stainless
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Stainless API key passed as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stainless-openapi.yml
  type: http
slug: stainless-authentication
source_filename: stainless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stainless-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Stainless API key passed as a Bearer token.\n  sources:\n  - openapi/stainless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/authentication/stainless-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Generation
- Documentation
- Developer Experience
- MCP
- Platform
- SDKs
- Terraform
---
