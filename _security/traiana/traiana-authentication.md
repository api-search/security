---
api_key_in:
- header
api_specs:
- filename: traiana-harmony-trade-processing-openapi.yml
  format: yaml
  label: Traiana Harmony Trade Processing API
  slug: harmony-trade-processing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-trade-processing-openapi.yml
- filename: traiana-harmony-creditlink-openapi.yml
  format: yaml
  label: Traiana Harmony CreditLink API
  slug: harmony-creditlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-creditlink-openapi.yml
- filename: traiana-harmony-netlink-openapi.yml
  format: yaml
  label: Traiana Harmony NetLink API
  slug: harmony-netlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-netlink-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Traiana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traiana secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Traiana
provider_slug: traiana
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/traiana-harmony-creditlink-openapi.yml
  - openapi/traiana-harmony-netlink-openapi.yml
  - openapi/traiana-harmony-trade-processing-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/traiana-harmony-creditlink-openapi.yml
  - openapi/traiana-harmony-netlink-openapi.yml
  - openapi/traiana-harmony-trade-processing-openapi.yml
  type: apiKey
slug: traiana-authentication
source_filename: traiana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/traiana-harmony-creditlink-openapi.yml, openapi/traiana-harmony-netlink-openapi.yml,\n  openapi/traiana-harmony-trade-processing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/traiana-harmony-creditlink-openapi.yml\n  - openapi/traiana-harmony-netlink-openapi.yml\n  - openapi/traiana-harmony-trade-processing-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/traiana-harmony-creditlink-openapi.yml\n  - openapi/traiana-harmony-netlink-openapi.yml\n  - openapi/traiana-harmony-trade-processing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/authentication/traiana-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
---
