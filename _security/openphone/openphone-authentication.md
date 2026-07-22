---
api_key_in:
- header
api_specs:
- filename: openphone-openapi-original.json
  format: json
  label: Quo Public API (OpenPhone)
  slug: quo-public-api-openphone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openphone/refs/heads/main/openapi/openphone-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Openphone Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenPhone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenPhone
provider_slug: openphone
scheme_count: 1
schemes:
- bearer: false
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/openphone-2026-03-30-openapi.json
  - openapi/openphone-openapi-original.json
  type: apiKey
slug: openphone-authentication
source_filename: openphone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/openphone-2026-03-30-openapi.json, openapi/openphone-openapi-original.json\ndocs: https://www.quo.com/docs/mdx/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\ndetails: >-\n  The Quo (OpenPhone) API uses API-key authentication. Include the API key in the\n  Authorization header of every request; it is sent verbatim and NOT as a Bearer\n  token. Keys are generated per-workspace under Settings > API by a workspace\n  owner or admin, carry full account privileges, and can be revoked individually.\n  Sending SMS to US numbers additionally requires completing US carrier\n  registration.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  bearer: false\n  sources:\n  - openapi/openphone-2026-03-30-openapi.json\n  - openapi/openphone-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openphone/refs/heads/main/authentication/openphone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Communications
- Voice
- SMS
- Messaging
- Telephony
- Business Phone
- CPaaS
- Contact Center
- Webhooks
---
