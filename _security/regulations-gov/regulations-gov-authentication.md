---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Regulations.gov API
  slug: regulations-gov-api
  spec_type: OpenAPI
  url: https://api.regulations.gov/v4/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Regulations Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regulations.gov secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Regulations.gov
provider_slug: regulations-gov
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/regulations-gov-regulations-gov-api-openapi.yml
  type: apiKey
slug: regulations-gov-authentication
source_filename: regulations-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regulations-gov-regulations-gov-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/regulations-gov-regulations-gov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/authentication/regulations-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Federal Rulemaking
- Public Comments
- Regulatory
- Dockets
- GSA
- Open Data
---
