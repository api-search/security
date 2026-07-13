---
api_key_in: []
api_specs:
- filename: llms.txt
  format: yaml
  label: Alloy Identity API
  slug: alloy-identity-api
  spec_type: OpenAPI
  url: https://developer.alloy.com/llms.txt
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alloy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alloy secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alloy
provider_slug: alloy
scheme_count: 2
schemes:
- description: HTTP basic authorization using a workflow token and secret
  name: basic
  scheme: basic
  sources:
  - openapi/alloy-identity-api-openapi.yml
  type: http
- description: OAuth2 using a workflow token and secret to generate a bearer token
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/bearer
  name: oauth2
  sources:
  - openapi/alloy-identity-api-openapi.yml
  type: oauth2
slug: alloy-authentication
source_filename: alloy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-identity-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: HTTP basic authorization using a workflow token and secret\n  sources:\n  - openapi/alloy-identity-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/bearer\n    scopes: 0\n  description: OAuth2 using a workflow token and secret to generate a bearer token\n  sources:\n  - openapi/alloy-identity-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/authentication/alloy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity Verification
- KYC
- KYB
- Fraud Prevention
- Compliance
- Onboarding
- Transaction Monitoring
- Risk Decisioning
- AML
- Fintech
---
