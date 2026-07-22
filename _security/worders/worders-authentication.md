---
api_key_in:
- cookie
api_specs:
- filename: worders-api-openapi-original.yml
  format: yaml
  label: Worders API V1
  slug: worders-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worders/refs/heads/main/openapi/worders-api-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Worders Authentication
name_suffix: Authentication
oauth_flows: []
overview: Worders secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Worders
provider_slug: worders
scheme_count: 2
schemes:
- description: Authenticated Devise session cookie (api.worders.net).
  in: cookie
  name: cookie_session
  parameter: _worders_session
  sources:
  - openapi/worders-api-openapi-original.yml
  type: apiKey
- description: 'Service API key issued from the admin UI. Sent as `Authorization: Bearer wrd_live_…`.'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/worders-api-openapi-original.yml
  type: http
slug: worders-authentication
source_filename: worders-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/worders-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookie_session\n  type: apiKey\n  in: cookie\n  parameter: _worders_session\n  description: Authenticated Devise session cookie (api.worders.net).\n  sources:\n  - openapi/worders-api-openapi-original.yml\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  description: 'Service API key issued from the admin UI. Sent as `Authorization: Bearer wrd_live_…`.'\n  sources:\n  - openapi/worders-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worders/refs/heads/main/authentication/worders-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Applicative Saas
- Localization
- Translation
- Culturalization
- Language Services
- Invoicing
---
