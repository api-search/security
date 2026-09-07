---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: edmunds-vehicle-api-openapi.yml
  format: yaml
  label: Edmunds Vehicle API
  slug: edmunds-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-vehicle-api-openapi.yml
- filename: edmunds-cars-openapi.yml
  format: yaml
  label: Edmunds Cars API
  slug: edmunds-cars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-cars-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Edmunds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edmunds secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Edmunds
provider_slug: edmunds
scheme_count: 2
schemes:
- applies_to: every documented Vehicle, Editorial, Dealer and Media API operation
  in: query
  name: ApiKeyAuth
  note: 'Documented as part of the URI template itself — {protocol}://api.edmunds.com/{endpoint}?fmt={format}&api_key={API key}. The dealership program page repeats it: "It is important that every URL you construct contains this key string otherwise no content will be returned." Because the credential travels in the query string it is exposed to browser history, proxy logs and Referer headers; Edmunds documents both http and https and only recommends https.'
  parameter: api_key
  required: true
  sources:
  - https://developer.edmunds.com/api-documentation/overview/
  - openapi/edmunds-vehicle-api-openapi.yml
  type: apiKey
- applies_to: the Edmunds Cars AI-plugin surface (/aiplugin/*)
  declared_in: https://api.edmunds.com/.well-known/ai-plugin.json
  name: AiPluginBearer
  note: The plugin manifest declares auth.type "service_http" with authorization_type "bearer". The OpenAPI that same manifest points at declares no securitySchemes and no security requirement at all, so the two first-party documents disagree about how this surface is authenticated. Recorded as published, not as verified — the surface could not be exercised.
  scheme: bearer
  type: http
slug: edmunds-authentication
source_filename: edmunds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://developer.edmunds.com/api-documentation/overview/ (URI Format),\n  https://developer.edmunds.com/dealership_api_program.html,\n  https://developer.edmunds.com/faq.html,\n  https://api.edmunds.com/.well-known/ai-plugin.json\ndocs: https://developer.edmunds.com/api-documentation/overview/\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - query\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  self_serve_signup: false\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: query\n    parameter: api_key\n    required: true\n    applies_to: every documented Vehicle, Editorial, Dealer and Media API operation\n    sources:\n      - https://developer.edmunds.com/api-documentation/overview/\n      - openapi/edmunds-vehicle-api-openapi.yml\n    note: >-\n      Documented as part of the URI template itself —\n      {protocol}://api.edmunds.com/{endpoint}?fmt={format}&api_key={API key}. The\n      dealership\
  \ program page repeats it: \"It is important that every URL you construct\n      contains this key string otherwise no content will be returned.\" Because the\n      credential travels in the query string it is exposed to browser history, proxy logs\n      and Referer headers; Edmunds documents both http and https and only recommends https.\n  - name: AiPluginBearer\n    type: http\n    scheme: bearer\n    declared_in: https://api.edmunds.com/.well-known/ai-plugin.json\n    applies_to: the Edmunds Cars AI-plugin surface (/aiplugin/*)\n    note: >-\n      The plugin manifest declares auth.type \"service_http\" with authorization_type\n      \"bearer\". The OpenAPI that same manifest points at declares no securitySchemes and no\n      security requirement at all, so the two first-party documents disagree about how this\n      surface is authenticated. Recorded as published, not as verified — the surface could\n      not be exercised.\nkey_issuance:\n  self_serve: false\n  status: closed\n\
  \  note: >-\n    Key issuance is closed. The open API program was retired effective 2018-02-15 and the\n    FAQ states Edmunds is \"not currently accepting new applicants\" and does \"not expect to\n    be able to accommodate new applicants in the future.\" Keys are issued only to select\n    strategic partners, service providers, dealers and automotive advertisers, and are\n    requested through an Edmunds Account Executive rather than through any signup form.\n  cross_ref: lifecycle/edmunds-lifecycle.yml\nobserved:\n  - url: https://api.edmunds.com/api/vehicle/v3/makes\n    status: 401\n    body_errorType: AUTHENTICATION_ERROR\n    body_message: Developer Inactive\n    checked: '2026-09-06'\n  - url: https://api.edmunds.com/aiplugin/curated-inventory/v1?zip=90401&pagenum=1&pagesize=3\n    status: 401\n    body_errorType: AUTHENTICATION_ERROR\n    body_message: Developer Inactive\n    checked: '2026-09-06'\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/authentication/edmunds-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Automobiles
- Cars
- Vehicles
- Vehicle Data
- Dealerships
- Reviews
- Pricing
- Automotive
---
