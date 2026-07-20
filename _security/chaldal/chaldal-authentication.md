---
api_key_in:
- header
api_specs:
- filename: chaldal-eggtransport-openapi-original.json
  format: json
  label: Chaldal Egg Transport (Gogo Bangla) Delivery API
  slug: chaldal-egg-transport-gogo-bangla-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaldal/refs/heads/main/openapi/chaldal-eggtransport-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chaldal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chaldal secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chaldal
provider_slug: chaldal
scheme_count: 2
schemes:
- description: Secret API key issued to the organization.
  in: header
  name: X-Egg-ApiKey
  parameter_name: X-Egg-ApiKey
  sources:
  - https://gogobangla.com/static/api-docs/
  type: apiKey
- description: User Id paired with the API key.
  in: header
  name: X-Egg-UserId
  parameter_name: X-Egg-UserId
  sources:
  - https://gogobangla.com/static/api-docs/
  type: apiKey
slug: chaldal-authentication
source_filename: chaldal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://gogobangla.com/static/api-docs/\ndocs: https://gogobangla.com/static/api-docs/\nnote: >-\n  The Egg Transport (Gogo Bangla) API uses header-based API-key authentication. Two secret\n  values must be sent on every request: the API key as X-Egg-ApiKey and the User Id as\n  X-Egg-UserId. The OpenAPI document itself declares no securitySchemes, so this profile is\n  captured from the published API reference rather than derived from the spec. Credentials are\n  issued on request by contacting tech@chaldal.com.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-Egg-ApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Egg-ApiKey\n  description: Secret API key issued to the organization.\n  sources:\n  - https://gogobangla.com/static/api-docs/\n- name: X-Egg-UserId\n  type: apiKey\n  in: header\n  parameter_name: X-Egg-UserId\n  description: User Id paired with the API key.\n\
  \  sources:\n  - https://gogobangla.com/static/api-docs/\nexample: >-\n  curl 'https://eggtransport.chaldal.com/api/Organization/GetOrgPickupPoints'\n  -H 'Accept: application/json'\n  -H 'X-Egg-ApiKey: 00000000-0000-0000-0000-000000000000'\n  -H 'X-Egg-UserId: 00000000-0000-0000-0000-000000000000'\ncredentials_contact: tech@chaldal.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaldal/refs/heads/main/authentication/chaldal-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Grocery
- Delivery
- Logistics
- Third Party Logistics
- Ecommerce
- Supply Chain
- Bangladesh
---
