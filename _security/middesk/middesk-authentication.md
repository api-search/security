---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Middesk Business Verification API
  slug: middesk-business-verification-api
  spec_type: OpenAPI
  url: https://docs.middesk.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Middesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Middesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Middesk
provider_slug: middesk
scheme_count: 1
schemes:
- name: bearer_auth
  scheme: bearer
  sources:
  - openapi/middesk-business-verification-openapi.yml
  type: http
slug: middesk-authentication
source_filename: middesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/middesk-business-verification-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/middesk-business-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/middesk/refs/heads/main/authentication/middesk-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Verification
- KYB
- Know Your Business
- Identity Verification
- Compliance
- EIN Validation
- TIN Verification
- Sanctions Screening
- Business Monitoring
- Fintech
- RegTech
---
