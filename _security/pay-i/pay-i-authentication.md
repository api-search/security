---
api_key_in:
- header
api_specs:
- filename: pay-i-openapi.yml
  format: yaml
  label: Pay-i API
  slug: pay-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pay I Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pay-i secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pay-i
provider_slug: pay-i
scheme_count: 1
schemes:
- description: 'Pay-I API Key. Example: "{apikey}"'
  in: header
  name: Pay_I_API_Key
  parameter: xProxy-api-key
  sources:
  - openapi/pay-i-openapi-original.json
  - openapi/pay-i-openapi.yml
  type: apiKey
slug: pay-i-authentication
source_filename: pay-i-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/pay-i-openapi-original.json, openapi/pay-i-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Pay_I_API_Key\n  type: apiKey\n  in: header\n  parameter: xProxy-api-key\n  description: 'Pay-I API Key. Example: \"{apikey}\"'\n  sources:\n  - openapi/pay-i-openapi-original.json\n  - openapi/pay-i-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/authentication/pay-i-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- FinOps
- Observability
- Cost Management
- Generative AI
- LLM
- Analytics
- Governance
- Metering
---
