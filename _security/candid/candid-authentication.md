---
api_key_in:
- header
api_specs:
- filename: candid-essentials-api-openapi.yml
  format: yaml
  label: Candid Essentials API
  slug: essentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid/refs/heads/main/openapi/candid-essentials-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Candid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Candid secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Candid
provider_slug: candid
scheme_count: 1
schemes:
- description: Candid subscription key required to call the Essentials API.
  in: header
  name: apiKeyAuth
  parameter: Subscription-Key
  sources:
  - openapi/candid-essentials-api-openapi.yml
  type: apiKey
slug: candid-authentication
source_filename: candid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/candid-essentials-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Subscription-Key\n  description: Candid subscription key required to call the Essentials API.\n  sources:\n  - openapi/candid-essentials-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid/refs/heads/main/authentication/candid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Charities
- Donations
- Non-Profits
- Philanthropy
- Foundations
- Grants
- 990s
- Demographics
---
