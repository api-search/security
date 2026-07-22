---
api_key_in:
- header
api_specs:
- filename: xeneta-api-30-openapi.yml
  format: yaml
  label: Xeneta API
  slug: xeneta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xeneta/refs/heads/main/openapi/xeneta-api-30-openapi.yml
auth_types:
- apiKey
- sessionCookie
description: 'The Xeneta API authenticates every request with an API key passed in the X-Auth header over HTTPS only — plain HTTP and unauthenticated requests are rejected. Keys are self-service generated in the Security section of the Xeneta account settings (https://app.xeneta.com/my-account/security) for accounts with API access. The separate airline reports API (Selfie) uses session-cookie authentication: POST username/password to /api/selfie/rest_auth/login on the airline host.'
kind: authentication
layout: security
method: searched
name: Xeneta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xeneta secures its APIs with apiKey and sessionCookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xeneta
provider_slug: xeneta
scheme_count: 2
schemes:
- https_required: true
  in: header
  key_source: https://app.xeneta.com/my-account/security
  name: sec0
  parameter: X-Auth
  sources:
  - openapi/xeneta-api-30-openapi.yml
  - https://help.xeneta.com/reference/authentication
  type: apiKey
- api: Xeneta Airline Data API
  credentials:
  - username
  - password
  login_endpoint: POST https://{airline}.useselfie.com/api/selfie/rest_auth/login
  name: airline-session
  sources:
  - https://help.xeneta.com/reference/airline-authentication
  type: sessionCookie
slug: xeneta-authentication
source_filename: xeneta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/xeneta-api-30-openapi.yml\ndocs: https://help.xeneta.com/reference/authentication\ndescription: >-\n  The Xeneta API authenticates every request with an API key passed in the\n  X-Auth header over HTTPS only — plain HTTP and unauthenticated requests are\n  rejected. Keys are self-service generated in the Security section of the\n  Xeneta account settings (https://app.xeneta.com/my-account/security) for\n  accounts with API access. The separate airline reports API (Selfie) uses\n  session-cookie authentication: POST username/password to\n  /api/selfie/rest_auth/login on the airline host.\nsummary:\n  types:\n  - apiKey\n  - sessionCookie\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Auth\n  key_source: https://app.xeneta.com/my-account/security\n  https_required: true\n  sources:\n  - openapi/xeneta-api-30-openapi.yml\n  - https://help.xeneta.com/reference/authentication\n\
  - name: airline-session\n  type: sessionCookie\n  api: Xeneta Airline Data API\n  login_endpoint: POST https://{airline}.useselfie.com/api/selfie/rest_auth/login\n  credentials: [username, password]\n  sources:\n  - https://help.xeneta.com/reference/airline-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xeneta/refs/heads/main/authentication/xeneta-authentication.yml
summary_line: apiKey/sessionCookie · 2 schemes
tags:
- Freight
- Shipping
- Logistics
- Ocean Freight
- Air Freight
- Benchmarking
- Market Data
- Supply Chain
- Rates
- Emissions
---
