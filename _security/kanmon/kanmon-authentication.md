---
api_key_in:
- header
api_specs:
- filename: kanmon-openapi-original.yml
  format: yaml
  label: Kanmon Public V2 API
  slug: kanmon-public-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kanmon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kanmon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kanmon
provider_slug: kanmon
scheme_count: 1
schemes:
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/kanmon-openapi-original.yml
  type: apiKey
slug: kanmon-authentication
source_filename: kanmon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kanmon-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/kanmon-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/authentication/kanmon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Embedded Finance
- Embedded Lending
- Lending
- Working Capital
- Invoice Financing
- API
---
