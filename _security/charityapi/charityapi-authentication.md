---
api_key_in:
- header
api_specs:
- filename: charityapi-openapi.yml
  format: yaml
  label: CharityAPI
  slug: charityapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/openapi/charityapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Charityapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CharityAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CharityAPI
provider_slug: charityapi
scheme_count: 1
schemes:
- description: API key issued by CharityAPI, sent in the apikey request header.
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/charityapi-openapi.yml
  type: apiKey
slug: charityapi-authentication
source_filename: charityapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charityapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key issued by CharityAPI, sent in the apikey request header.\n  sources:\n  - openapi/charityapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/authentication/charityapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- 501c3
- Charities
- Donations
- EIN
- IRS
- Non-Profits
- Tax Compliance
- Verification
---
