---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fsmacrypto-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: FSMA Crypto Promotions Checker Enquiry API
  slug: fsmacrypto-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fsmacrypto-co-uk/openapi/fsmacrypto-co-uk-enquiry-api-openapi.yml
- filename: fsmacrypto-co-uk-guide-api-openapi.yml
  format: yaml
  label: FSMA Crypto Promotions Checker Guide API
  slug: fsmacrypto-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fsmacrypto-co-uk/openapi/fsmacrypto-co-uk-guide-api-openapi.yml
- filename: fsmacrypto-co-uk-mcp-api-openapi.yml
  format: yaml
  label: FSMA Crypto Promotions Checker MCP API
  slug: fsmacrypto-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fsmacrypto-co-uk/openapi/fsmacrypto-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FSMA Crypto Promotions Checker Authentication
name_suffix: Authentication
oauth_flows: []
overview: FSMA Crypto Promotions Checker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FSMA Crypto Promotions Checker
provider_slug: fsmacrypto-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/fsmacrypto-co-uk-openapi.json
  type: http
slug: fsmacrypto-co-uk-authentication
source_filename: fsmacrypto-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/fsmacrypto-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/fsmacrypto-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fsmacrypto-co-uk/authentication/fsmacrypto-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- FCA
- United Kingdom
- Financial-Promotion
- Compliance
---
