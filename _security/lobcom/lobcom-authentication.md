---
api_key_in: []
api_specs:
- filename: lobcom-openapi-original.yml
  format: yaml
  label: Lob API
  slug: lobcom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lobcom/refs/heads/main/openapi/lobcom-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lobcom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lob.com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lob.com
provider_slug: lobcom
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/lobcom-openapi-original.yml
  type: http
slug: lobcom-authentication
source_filename: lobcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/lobcom-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lobcom-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lobcom/refs/heads/main/authentication/lobcom-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Direct Mail
- Print
- Address Verification
- Mail
- Postcards
- Letters
- Checks
- Campaigns
- USPS
- Deliverability
---
