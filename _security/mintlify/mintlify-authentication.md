---
api_key_in: []
api_specs:
- filename: mintlify-agent-api-openapi.yml
  format: yaml
  label: Mintlify Agent API
  slug: mintlify-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-agent-api-openapi.yml
- filename: mintlify-analytics-api-openapi.yml
  format: yaml
  label: Mintlify Analytics API
  slug: mintlify-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-analytics-api-openapi.yml
- filename: mintlify-assistant-api-openapi.yml
  format: yaml
  label: Mintlify Assistant API
  slug: mintlify-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-assistant-api-openapi.yml
- filename: mintlify-update-api-openapi.yml
  format: yaml
  label: Mintlify Update API
  slug: mintlify-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-update-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mintlify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mintlify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mintlify
provider_slug: mintlify
scheme_count: 1
schemes:
- bearerFormat: mint_*
  description: Admin API key prefixed with mint_.
  name: adminKey
  scheme: bearer
  sources:
  - openapi/mintlify-openapi.yml
  type: http
slug: mintlify-authentication
source_filename: mintlify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mintlify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: adminKey\n  type: http\n  scheme: bearer\n  bearerFormat: mint_*\n  description: Admin API key prefixed with mint_.\n  sources:\n  - openapi/mintlify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/authentication/mintlify-authentication.yml
summary_line: http · 1 scheme
tags:
- Documentation
---
