---
api_key_in:
- header
api_specs:
- filename: laka-platform-openapi.json
  format: json
  label: Laka Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/openapi/laka-platform-openapi.json
- filename: laka-quote-openapi.json
  format: json
  label: Laka Quote API
  slug: quote
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/openapi/laka-quote-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Laka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laka secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Laka
provider_slug: laka
scheme_count: 2
schemes:
- api: Laka Platform API
  applied_to: 38 of 39 published Platform operations
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/laka-platform-openapi.json
  type: apiKey
- api: Laka Quote API
  applied_to: 18 of 19 published Quote operations
  description: Secures endpoint by requiring an API key.
  in: header
  name: api_key_header_Authorization
  note: 'Despite the header name, this is a plain API key rather than an OAuth bearer token — the published securityScheme is type apiKey, not http/bearer. Laka''s own documented header example sends it as `Authorization: YOUR_TOKEN`.'
  parameter: Authorization
  sources:
  - openapi/laka-quote-openapi.json
  type: apiKey
slug: laka-authentication
source_filename: laka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/laka-platform-openapi.json, openapi/laka-quote-openapi.json\ndocs:\n- https://docs.laka.co/docs/regions\n- https://docs.laka.co/docs/request-access\n- https://docs.laka.co/docs/glossary\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  note: 'Laka is API-key based end to end. There is no authorization server, token endpoint, refresh\n    flow or scope surface — /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return 404 on every Laka host. The two APIs use different\n    header names, which is the single most common integration mistake: the Platform API reads\n    x-api-key while the Quote API reads Authorization.'\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  api: Laka Platform API\n  applied_to: 38 of 39 published Platform operations\n  sources:\n  - openapi/laka-platform-openapi.json\n\
  - name: api_key_header_Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Secures endpoint by requiring an API key.\n  api: Laka Quote API\n  applied_to: 18 of 19 published Quote operations\n  note: 'Despite the header name, this is a plain API key rather than an OAuth bearer token — the\n    published securityScheme is type apiKey, not http/bearer. Laka''s own documented header example\n    sends it as `Authorization: YOUR_TOKEN`.'\n  sources:\n  - openapi/laka-quote-openapi.json\nrequired_companion_headers:\n- name: x-api-region\n  required: true\n  description: 'The API region of the interaction; in most cases it matches the customer region. Laka\n    uses it to attribute the insured party to the correct regulatory region.'\n  documented_values: [gb, nl, be, de, fr, dk, at, ie]\n- name: x-api-language\n  required: true\n  description: Where applicable, the language for any textual content Laka may send to the customer.\n  documented_values: [en,\
  \ nl, fr, de, dk]\ndocumented_header_example:\n  Content-Type: application/json\n  x-api-region: be\n  x-api-language: nl\n  x-api-key: YOUR_KEY\n  Authorization: YOUR_TOKEN\n  source: https://docs.laka.co/docs/regions\ncredential_issuance:\n  self_service: false\n  model: 'Access is granted per partner. Laka asks prospective partners to request API access by\n    email; there is no developer signup that mints a key.'\n  url: https://docs.laka.co/docs/request-access\ntransport:\n  https_required: true\n  hsts: true\n  note: 'Laka states all traffic and requests must be over HTTPS; probed hosts return\n    strict-transport-security max-age=31536000 includeSubDomains.'\nrotation:\n  documented: false\n  note: No key rotation, expiry or revocation procedure is published on the developer surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/authentication/laka-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Insurance
- InsurTech
- Cycling
- Micro Mobility
- Bicycle Insurance
- Claims
- Policies
- Quotes
- Embedded Insurance
- Europe
---
