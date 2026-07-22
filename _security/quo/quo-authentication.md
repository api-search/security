---
api_key_in:
- header
api_specs:
- filename: quo-public-api-v1.json
  format: json
  label: Quo Public API
  slug: quo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quo/refs/heads/main/openapi/quo-public-api-v1.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Quo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quo
provider_slug: quo
scheme_count: 1
schemes:
- bearer: false
  in: header
  name: apiKey
  note: Send the raw API key as the Authorization header value; the Quo API does NOT use a Bearer token prefix. Keys are generated in workspace Settings > API by an owner or admin, are named (no spaces), and grant full workspace access. Rotate regularly and revoke compromised keys from workspace settings.
  parameter: Authorization
  sources:
  - openapi/quo-public-api-v1.json
  - https://www.quo.com/docs/mdx/api-reference/authentication
  type: apiKey
slug: quo-authentication
source_filename: quo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quo-public-api-v1.json\ndocs: https://www.quo.com/docs/mdx/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  bearer: false\n  note: >-\n    Send the raw API key as the Authorization header value; the Quo API does NOT\n    use a Bearer token prefix. Keys are generated in workspace Settings > API by\n    an owner or admin, are named (no spaces), and grant full workspace access.\n    Rotate regularly and revoke compromised keys from workspace settings.\n  sources:\n  - openapi/quo-public-api-v1.json\n  - https://www.quo.com/docs/mdx/api-reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quo/refs/heads/main/authentication/quo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Communication
- Messaging
- SMS
- Voice
- Contacts
- Webhooks
- API
---
