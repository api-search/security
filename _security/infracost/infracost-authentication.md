---
api_key_in:
- header
api_specs:
- filename: infracost-openapi.yml
  format: yaml
  label: Infracost Cloud Pricing API
  slug: infracost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infracost/refs/heads/main/openapi/infracost-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Infracost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infracost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infracost
provider_slug: infracost
scheme_count: 1
schemes:
- description: Infracost API key
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/infracost-openapi.yml
  type: apiKey
slug: infracost-authentication
source_filename: infracost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infracost-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Infracost API key\n  sources:\n  - openapi/infracost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infracost/refs/heads/main/authentication/infracost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Cost
- FinOps
- Infrastructure
- Terraform
---
