---
api_key_in: []
api_specs:
- filename: nango-openapi.yml
  format: yaml
  label: Nango
  slug: nango
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nango/refs/heads/main/openapi/nango-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nango Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nango secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nango
provider_slug: nango
scheme_count: 1
schemes:
- description: Nango secret key supplied as a bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nango-openapi.yml
  type: http
slug: nango-authentication
source_filename: nango-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nango-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Nango secret key supplied as a bearer token.\n  sources:\n  - openapi/nango-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nango/refs/heads/main/authentication/nango-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Integrations
- OAuth
- Syncing
- Unified API
- Webhooks
---
