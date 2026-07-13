---
api_key_in: []
api_specs:
- filename: alloy-openapi.yml
  format: yaml
  label: Alloy API
  slug: alloy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alloy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloy secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alloy
provider_slug: alloy
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with workflow or account-level API key as username and secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/alloy-openapi.yml
  type: http
- description: OAuth 2.0 bearer token obtained via the OAuth endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alloy-openapi.yml
  type: http
slug: alloy-com-authentication
source_filename: alloy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with workflow or account-level API key as username\n    and secret as password.\n  sources:\n  - openapi/alloy-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token obtained via the OAuth endpoints.\n  sources:\n  - openapi/alloy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/authentication/alloy-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Decisioning
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Credit Underwriting
- Ongoing Monitoring
- Case Management
- Fintech
- Banking
---
