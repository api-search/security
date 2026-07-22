---
api_key_in:
- header
api_specs:
- filename: orderly-health-provider-directory-openapi.json
  format: json
  label: Orderly Provider Directory API
  slug: orderly-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-health/refs/heads/main/openapi/orderly-health-provider-directory-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orderly Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orderly Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orderly Health
provider_slug: orderly-health
scheme_count: 1
schemes:
- in: header
  name: OrderlyAPIToken
  parameter: Authorization
  sources:
  - openapi/orderly-health-provider-directory-openapi.json
  type: apiKey
slug: orderly-health-authentication
source_filename: orderly-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orderly-health-provider-directory-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OrderlyAPIToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/orderly-health-provider-directory-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderly-health/refs/heads/main/authentication/orderly-health-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Provider Data
- Provider Directory
- Health Data
- Machine Learning
- Data Quality
- Interoperability
---
