---
api_key_in:
- header
api_specs:
- filename: huuray-openapi.yml
  format: yaml
  label: Huuray Gift Card API
  slug: huuray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huuray/refs/heads/main/openapi/huuray-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Huuray Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huuray secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Huuray
provider_slug: huuray
scheme_count: 1
schemes:
- description: The API-Token provided to you by Huuray.
  in: header
  name: ApiToken
  parameter: X-API-TOKEN
  sources:
  - openapi/huuray-openapi.yml
  type: apiKey
slug: huuray-authentication
source_filename: huuray-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/huuray-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  description: The API-Token provided to you by Huuray.\n  sources:\n  - openapi/huuray-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huuray/refs/heads/main/authentication/huuray-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Commerce
- Gift Cards
- Payments
- Rewards
---
