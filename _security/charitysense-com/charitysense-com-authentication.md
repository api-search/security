---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: charitysense-com-openapi.yml
  format: yaml
  label: CharitySense Data API
  slug: charitysense-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/openapi/charitysense-com-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Charitysense Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CharitySense secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CharitySense
provider_slug: charitysense-com
scheme_count: 2
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/charitysense-com-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-CharitySense-API-Key
  sources:
  - openapi/charitysense-com-openapi.yml
  type: apiKey
slug: charitysense-com-authentication
source_filename: charitysense-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/charitysense-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/charitysense-com-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CharitySense-API-Key\n  sources:\n  - openapi/charitysense-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/authentication/charitysense-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Non-Profit
- Charities
- Due Diligence
- IRS Form 990
- Donor Research
- Grants
- Philanthropy
- Open Data
- Agents
- A2A
- Impact Verification
- Edge AI
- United States
- Company
---
