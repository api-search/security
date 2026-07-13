---
api_key_in:
- header
api_specs:
- filename: agechecker-net-age-verification-openapi.yml
  format: yaml
  label: AgeChecker.Net Age Verification API
  slug: agechecker-net-age-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/openapi/agechecker-net-age-verification-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agechecker Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgeChecker.Net secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgeChecker.Net
provider_slug: agechecker-net
scheme_count: 1
schemes:
- description: API key for AgeChecker.Net API access.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/agechecker-net-age-verification-openapi.yml
  type: apiKey
slug: agechecker-net-authentication
source_filename: agechecker-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agechecker-net-age-verification-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for AgeChecker.Net API access.\n  sources:\n  - openapi/agechecker-net-age-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/authentication/agechecker-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
---
