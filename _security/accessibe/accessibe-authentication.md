---
api_key_in:
- header
api_specs:
- filename: accessibe-accounts-api-openapi.yml
  format: yaml
  label: accessiBe Accounts API
  slug: accessibe-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accessibe/refs/heads/main/openapi/accessibe-accounts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Accessibe Authentication
name_suffix: Authentication
oauth_flows: []
overview: accessiBe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: accessiBe
provider_slug: accessibe
scheme_count: 1
schemes:
- description: API key generated for the account
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/accessibe-partners-openapi-original.yml
  type: apiKey
slug: accessibe-authentication
source_filename: accessibe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/accessibe-partners-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key generated for the account\n  sources:\n  - openapi/accessibe-partners-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessibe/refs/heads/main/authentication/accessibe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Accessibility
- Web Accessibility
- WCAG
- ADA Compliance
- Compliance
- Developer Tools
- Testing
- Quality Assurance
- Artificial Intelligence
---
