---
api_key_in:
- header
api_specs:
- filename: passbase-verification-openapi.yml
  format: yaml
  label: Passbase Verifications API
  slug: passbase-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passbase/refs/heads/main/openapi/passbase-verification-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Passbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Passbase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Passbase
provider_slug: passbase
scheme_count: 1
schemes:
- description: Secret API key sent in the X-API-KEY header. A Bearer JWT (identity_access_token) may also be supplied by prefixing the header value with "Bearer ".
  in: header
  name: SecuredKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/passbase-verification-openapi.yml
  type: apiKey
slug: passbase-authentication
source_filename: passbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/passbase-verification-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SecuredKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Secret API key sent in the X-API-KEY header. A Bearer JWT (identity_access_token)\n    may also be supplied by prefixing the header value with \"Bearer \".\n  sources:\n  - openapi/passbase-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passbase/refs/heads/main/authentication/passbase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Identity Verification
- KYC
- Biometrics
- Authentication
- Identity
- Compliance
---
