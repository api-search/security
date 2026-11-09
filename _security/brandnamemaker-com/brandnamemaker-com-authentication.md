---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: brandnamemaker-com-hero-api-openapi.yml
  format: yaml
  label: True Frontier Hero API
  slug: brandnamemaker-com-hero-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brandnamemaker-com/openapi/brandnamemaker-com-hero-api-openapi.yml
- filename: brandnamemaker-com-name-api-openapi.yml
  format: yaml
  label: True Frontier Name API
  slug: brandnamemaker-com-name-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brandnamemaker-com/openapi/brandnamemaker-com-name-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Brandnamemaker Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: True Frontier secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: True Frontier
provider_slug: brandnamemaker-com
scheme_count: 3
schemes:
- description: 'MPP credential from the runtime WWW-Authenticate: Payment challenge.'
  name: payment
  scheme: Payment
  sources:
  - openapi/brandnamemaker-com-openapi.json
  type: http
- description: Legacy Base x402 credential.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/brandnamemaker-com-openapi.json
  type: apiKey
- in: header
  name: x402Legacy
  parameter: X-PAYMENT
  sources:
  - openapi/brandnamemaker-com-openapi.json
  type: apiKey
slug: brandnamemaker-com-authentication
source_filename: brandnamemaker-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/brandnamemaker-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: payment\n  type: http\n  scheme: Payment\n  description: 'MPP credential from the runtime WWW-Authenticate: Payment challenge.'\n  sources:\n  - openapi/brandnamemaker-com-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Legacy Base x402 credential.\n  sources:\n  - openapi/brandnamemaker-com-openapi.json\n- name: x402Legacy\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  sources:\n  - openapi/brandnamemaker-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/brandnamemaker-com/authentication/brandnamemaker-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artificial Intelligence
- Naming
- Branding
- DomainCheck
---
