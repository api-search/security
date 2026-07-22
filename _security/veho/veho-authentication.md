---
api_key_in:
- header
api_specs:
- filename: veho-api-openapi-original.yml
  format: yaml
  label: Veho API
  slug: veho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veho/refs/heads/main/openapi/veho-api-openapi-original.yml
auth_types:
- apiKey
description: The Veho API authenticates with a static API key provided by Veho, sent on every request in an `apikey` header (UUID-shaped in the docs example). Sandbox and production use separate keys and hosts. 401 means the header was missing or the key invalid; 403 means the key lacks permission for the requested resource. GET /serviceable-zips on the sandbox host is the only documented unauthenticated endpoint. No OAuth, OIDC, or mTLS surface.
kind: authentication
layout: security
method: searched
name: Veho Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veho secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veho
provider_slug: veho
scheme_count: 1
schemes:
- errors:
    '401': missing or invalid apikey header
    '403': apikey lacks permission for the requested resource
  in: header
  name: apiKey
  parameter: apikey
  provisioning: API keys are issued by Veho (sales/integration-led); separate key per environment
  sources:
  - openapi/veho-api-openapi-original.yml
  type: apiKey
slug: veho-authentication
source_filename: veho-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/veho-api-openapi-original.yml\ndocs: https://docs.api.shipveho.com/docs/veho-api/jn0u5escxmisw-authentication\ndescription: >-\n  The Veho API authenticates with a static API key provided by Veho, sent on\n  every request in an `apikey` header (UUID-shaped in the docs example).\n  Sandbox and production use separate keys and hosts. 401 means the header\n  was missing or the key invalid; 403 means the key lacks permission for the\n  requested resource. GET /serviceable-zips on the sandbox host is the only\n  documented unauthenticated endpoint. No OAuth, OIDC, or mTLS surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  provisioning: API keys are issued by Veho (sales/integration-led); separate key per environment\n  errors:\n    '401': missing or invalid apikey header\n    '403': apikey lacks permission for the requested resource\n\
  \  sources:\n  - openapi/veho-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veho/refs/heads/main/authentication/veho-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Last Mile Delivery
- Package Tracking
- eCommerce
- Webhooks
- Delivery
---
