---
api_key_in:
- header
api_specs:
- filename: trustwell-foodlogiq-openapi.yml
  format: yaml
  label: Trustwell FoodLogiQ API
  slug: trustwell-foodlogiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustwell/refs/heads/main/openapi/trustwell-foodlogiq-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trustwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trustwell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trustwell
provider_slug: trustwell
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/trustwell-foodlogiq-openapi.yml
  type: apiKey
slug: trustwell-authentication
source_filename: trustwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trustwell-foodlogiq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/trustwell-foodlogiq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustwell/refs/heads/main/authentication/trustwell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food Industry
- Food Safety
- Nutrition
- Supply Chain
- Food Labeling
- Traceability
- Compliance
- Food Technology
---
