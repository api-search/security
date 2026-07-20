---
api_key_in:
- header
api_specs:
- filename: airspace-technologies-v3-openapi.json
  format: json
  label: Airspace API V3
  slug: airspace-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/openapi/airspace-technologies-v3-openapi.json
- filename: airspace-technologies-v2-openapi.json
  format: json
  label: Airspace API V2
  slug: airspace-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/openapi/airspace-technologies-v2-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Airspace Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airspace Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airspace Technologies
provider_slug: airspace-technologies
scheme_count: 1
schemes:
- description: 'Unique API key necessary to make API requests. Sent as Authorization: Bearer <API_KEY> header.'
  header: Authorization
  in: header
  name: Bearer
  scheme: bearer
  sources:
  - openapi/airspace-technologies-v2-openapi.json
  - openapi/airspace-technologies-v3-openapi.json
  type: http
slug: airspace-technologies-authentication
source_filename: airspace-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/airspace-technologies-v2-openapi.json, openapi/airspace-technologies-v3-openapi.json\ndocs: https://api.airspace.com/api-docs/v3\nsummary:\n  types:\n  - http\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: 'Unique API key necessary to make API requests. Sent as Authorization: Bearer <API_KEY> header.'\n  sources:\n  - openapi/airspace-technologies-v2-openapi.json\n  - openapi/airspace-technologies-v3-openapi.json\nnotes:\n- API tokens are provisioned by Airspace, not self-service. Contact integrations@airspace.com to request a key.\n- Once issued, a token does not expire.\n- New integrators are provisioned against the test environment (apitest.airspace.com) first; production access is enabled after end-to-end testing sign-off.\n- No OAuth2 scope surface; access is account-scoped by the issued bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/authentication/airspace-technologies-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Freight
- Supply Chain
- Transportation
- Webhooks
- Orders
---
