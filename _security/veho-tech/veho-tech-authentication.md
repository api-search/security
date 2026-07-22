---
api_key_in:
- header
api_specs:
- filename: veho-tech-api-openapi-original.yml
  format: yaml
  label: Veho API
  slug: veho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veho-tech/refs/heads/main/openapi/veho-tech-api-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Veho Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veho Tech secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veho Tech
provider_slug: veho-tech
scheme_count: 1
schemes:
- in: header
  name: apiKey
  notes: 'UUID-format key sent as `apikey: 00000000-0000-0000-0000-000000000000` (docs placeholder example). Applied globally to all operations.'
  parameter: apikey
  sources:
  - openapi/veho-tech-api-openapi-original.yml
  type: apiKey
slug: veho-tech-authentication
source_filename: veho-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/veho-tech-api-openapi-original.yml\ndocs: https://docs.api.shipveho.com/docs/veho-api/jn0u5escxmisw-authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/veho-tech-api-openapi-original.yml\n  notes: >-\n    UUID-format key sent as `apikey: 00000000-0000-0000-0000-000000000000`\n    (docs placeholder example). Applied globally to all operations.\nprovisioning: >-\n  API keys are provided by Veho — there is no self-serve signup. Sandbox and\n  production environments use separate keys; contact api@shipveho.com.\nerror_semantics:\n  '401': Unauthorized — request missing an `apikey` header, or the key was invalid.\n  '403': Forbidden — the key doesn't have permission for the requested resource.\nunauthenticated_endpoints:\n- GET /serviceable-zips on the sandbox host (per Sandbox Environment docs)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veho-tech/refs/heads/main/authentication/veho-tech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Logistics
- Shipping
- Last-Mile Delivery
- Package Tracking
- E-Commerce
- Delivery
- Webhooks
---
