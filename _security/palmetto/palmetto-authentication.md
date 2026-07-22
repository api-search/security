---
api_key_in:
- header
api_specs:
- filename: palmetto-energy-intelligence-openapi.json
  format: json
  label: Palmetto Energy Intelligence API
  slug: palmetto-energy-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palmetto/refs/heads/main/openapi/palmetto-energy-intelligence-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Palmetto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palmetto secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Palmetto
provider_slug: palmetto
scheme_count: 3
schemes:
- docs: https://docs.palmetto.com/ei-api/overview/
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  product: Energy Intelligence
  sources:
  - openapi/palmetto-energy-intelligence-openapi.json
  type: apiKey
- docs: https://docs.palmetto.com/energy/environments/
  login_endpoint: POST https://api.palmetto.com/api/v1/auth/login
  login_endpoint_next: POST https://api-next.palmetto.com/api/v1/auth/login
  name: BearerLogin
  product: Energy Platform
  request: '{ "username": "string", "password": "string" }'
  response_fields:
  - access_token
  - expires_in
  - refresh_token
  - token_type
  scheme: bearer
  sources:
  - https://docs.palmetto.com/energy/getting-started/
  token_type: Bearer
  type: http
- docs: https://docs.palmetto.com/finance/getting-started/
  identity: machine-to-machine (M2M) user; cannot sign in to the portal
  login_endpoint: POST ${envBaseUrl}/api/auth/login
  name: BearerLoginM2M
  product: Finance (LightReach)
  request: '{ "username": "string", "password": "string" }'
  response_fields:
  - access_token
  - expires_in
  - refresh_token
  - token_type
  scheme: bearer
  sources:
  - https://docs.palmetto.com/finance/getting-started/
  token_type: Bearer
  type: http
slug: palmetto-authentication
source_filename: palmetto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/palmetto-energy-intelligence-openapi.json\ndocs: https://docs.palmetto.com/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Palmetto ships three developer products with two distinct auth models.\n    Energy Intelligence uses a static API key sent in the X-API-Key header.\n    The Energy Platform and Finance (LightReach) APIs use bearer tokens\n    obtained from a username/password login endpoint (machine-to-machine\n    users), cached until expiry and refreshed via the login/refresh flow.\nschemes:\n- name: APIKeyHeader\n  product: Energy Intelligence\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  docs: https://docs.palmetto.com/ei-api/overview/\n  sources:\n  - openapi/palmetto-energy-intelligence-openapi.json\n- name: BearerLogin\n  product: Energy Platform\n  type: http\n  scheme: bearer\n  token_type: Bearer\n  login_endpoint: POST https://api.palmetto.com/api/v1/auth/login\n\
  \  login_endpoint_next: POST https://api-next.palmetto.com/api/v1/auth/login\n  request: '{ \"username\": \"string\", \"password\": \"string\" }'\n  response_fields: [access_token, expires_in, refresh_token, token_type]\n  docs: https://docs.palmetto.com/energy/environments/\n  sources:\n  - https://docs.palmetto.com/energy/getting-started/\n- name: BearerLoginM2M\n  product: Finance (LightReach)\n  type: http\n  scheme: bearer\n  token_type: Bearer\n  login_endpoint: POST ${envBaseUrl}/api/auth/login\n  request: '{ \"username\": \"string\", \"password\": \"string\" }'\n  response_fields: [access_token, expires_in, refresh_token, token_type]\n  identity: machine-to-machine (M2M) user; cannot sign in to the portal\n  docs: https://docs.palmetto.com/finance/getting-started/\n  sources:\n  - https://docs.palmetto.com/finance/getting-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palmetto/refs/heads/main/authentication/palmetto-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Clean Energy
- Solar
- Energy
- Building Energy Modeling
- Home Energy
- Financing
- Sustainability
---
