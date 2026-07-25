---
api_key_in:
- header
api_specs:
- filename: traiana-allocations-api-openapi.yml
  format: yaml
  label: Traiana Allocations API
  slug: traiana-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-allocations-api-openapi.yml
- filename: traiana-compression-api-openapi.yml
  format: yaml
  label: Traiana Compression API
  slug: traiana-compression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-compression-api-openapi.yml
- filename: traiana-credit-limits-api-openapi.yml
  format: yaml
  label: Traiana Credit Limits API
  slug: traiana-credit-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-credit-limits-api-openapi.yml
- filename: traiana-designation-notices-api-openapi.yml
  format: yaml
  label: Traiana Designation Notices API
  slug: traiana-designation-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-designation-notices-api-openapi.yml
- filename: traiana-give-ups-api-openapi.yml
  format: yaml
  label: Traiana Give-Ups API
  slug: traiana-give-ups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-give-ups-api-openapi.yml
- filename: traiana-matching-api-openapi.yml
  format: yaml
  label: Traiana Matching API
  slug: traiana-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-matching-api-openapi.yml
- filename: traiana-netting-api-openapi.yml
  format: yaml
  label: Traiana Netting API
  slug: traiana-netting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-netting-api-openapi.yml
- filename: traiana-settlement-api-openapi.yml
  format: yaml
  label: Traiana Settlement API
  slug: traiana-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-settlement-api-openapi.yml
- filename: traiana-trades-api-openapi.yml
  format: yaml
  label: Traiana Trades API
  slug: traiana-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-trades-api-openapi.yml
- filename: traiana-utilization-api-openapi.yml
  format: yaml
  label: Traiana Utilization API
  slug: traiana-utilization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-utilization-api-openapi.yml
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
