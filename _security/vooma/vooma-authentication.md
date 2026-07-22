---
api_key_in: []
api_specs:
- filename: vooma-openapi-original.json
  format: json
  label: Vooma Public API
  slug: vooma-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vooma/refs/heads/main/openapi/vooma-openapi-original.json
auth_types:
- http
description: Auth profile for the Vooma Public API. All 25 REST operations require the "bearer" scheme — an organization API key sent as a bearer token (bearerFormat "API Key"). API keys are created by an organization admin in the Vooma app and require an enterprise license. The spec also defines a basic scheme and an "auth0" bearer JWT scheme (Auth0-issued user tokens for the app), but no public operation references them. Webhook callbacks Vooma sends to your server declare no security scheme in the spec.
kind: authentication
layout: security
method: searched
name: Vooma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vooma secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vooma
provider_slug: vooma
scheme_count: 3
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/vooma-openapi-original.json
  type: http
- bearerFormat: API Key
  description: Organization API key sent as a bearer token; used by all 25 public operations.
  name: bearer
  scheme: bearer
  sources:
  - openapi/vooma-openapi-original.json
  type: http
- bearerFormat: JWT
  description: Auth0-issued JWT; defined in components.securitySchemes but not referenced by any public operation.
  name: auth0
  scheme: bearer
  sources:
  - openapi/vooma-openapi-original.json
  type: http
slug: vooma-authentication
source_filename: vooma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/vooma-openapi-original.json\ndocs: https://docs.vooma.ai/api-reference/introduction\ndescription: >-\n  Auth profile for the Vooma Public API. All 25 REST operations require the\n  \"bearer\" scheme — an organization API key sent as a bearer token\n  (bearerFormat \"API Key\"). API keys are created by an organization admin in\n  the Vooma app and require an enterprise license. The spec also defines a\n  basic scheme and an \"auth0\" bearer JWT scheme (Auth0-issued user tokens for\n  the app), but no public operation references them. Webhook callbacks Vooma\n  sends to your server declare no security scheme in the spec.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  api_key_style: bearer token (bearerFormat \"API Key\")\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/vooma-openapi-original.json\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ API Key\n  description: Organization API key sent as a bearer token; used by all 25 public operations.\n  sources:\n  - openapi/vooma-openapi-original.json\n- name: auth0\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Auth0-issued JWT; defined in components.securitySchemes but not referenced by any public operation.\n  sources:\n  - openapi/vooma-openapi-original.json\nnotes:\n- You must be an organization admin to create an API key.\n- An enterprise license is required to develop against the Vooma Public API.\n- 'Support contact for auth failures: support@vooma.ai'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vooma/refs/heads/main/authentication/vooma-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- AI
- Freight
- Logistics
- Transportation
- Brokers
- TMS
- Agents
---
