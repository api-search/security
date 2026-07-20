---
api_key_in:
- header
api_specs:
- filename: aqueduct-openapi.json
  format: json
  label: Aqueduct API
  slug: aqueduct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aqueduct Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aqueduct secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aqueduct
provider_slug: aqueduct
scheme_count: 1
schemes:
- format: Api-Key {key}
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/aqueduct-openapi.json
  type: apiKey
slug: aqueduct-authentication
source_filename: aqueduct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aqueduct-openapi.json\ndocs: https://docs.tryaqueduct.com/reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Aqueduct authenticates every request with an API key issued from the dashboard\n  (dashboard.tryaqueduct.com settings page). The key is sent in the Authorization\n  header using the literal prefix \"Api-Key\", i.e. `Authorization: Api-Key {key}`.\n  All requests must be made over HTTPS. There is no OAuth surface. The OpenAPI\n  models this as an apiKey scheme (named \"bearerAuth\" in the spec) in the\n  Authorization header.\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Api-Key {key}'\n  sources:\n  - openapi/aqueduct-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/authentication/aqueduct-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Billing
- Invoicing
- Metering
- Usage-Based
- Subscriptions
- Payments
- API
---
