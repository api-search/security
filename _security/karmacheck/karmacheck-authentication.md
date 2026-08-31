---
api_key_in: []
api_specs:
- filename: karmacheck-authentication-api-openapi.yml
  format: yaml
  label: KarmaCheck Authentication API
  slug: karmacheck-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-authentication-api-openapi.yml
- filename: karmacheck-candidate-onboarding-api-openapi.yml
  format: yaml
  label: KarmaCheck Candidate onboarding API
  slug: karmacheck-candidate-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-candidate-onboarding-api-openapi.yml
- filename: karmacheck-case-api-openapi.yml
  format: yaml
  label: KarmaCheck Case API
  slug: karmacheck-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-case-api-openapi.yml
- filename: karmacheck-cases-api-openapi.yml
  format: yaml
  label: KarmaCheck Cases API
  slug: karmacheck-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-cases-api-openapi.yml
- filename: karmacheck-packages-api-openapi.yml
  format: yaml
  label: KarmaCheck Packages API
  slug: karmacheck-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-packages-api-openapi.yml
- filename: karmacheck-secure-documents-api-openapi.yml
  format: yaml
  label: KarmaCheck Secure documents API
  slug: karmacheck-secure-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-secure-documents-api-openapi.yml
- filename: karmacheck-services-api-openapi.yml
  format: yaml
  label: KarmaCheck Services API
  slug: karmacheck-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-services-api-openapi.yml
- filename: karmacheck-users-api-openapi.yml
  format: yaml
  label: KarmaCheck Users API
  slug: karmacheck-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-users-api-openapi.yml
- filename: karmacheck-verification-book-api-openapi.yml
  format: yaml
  label: KarmaCheck Verification Book API
  slug: karmacheck-verification-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-verification-book-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Karmacheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: KarmaCheck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KarmaCheck
provider_slug: karmacheck
scheme_count: 1
schemes:
- name: JWT
  scheme: bearer
  sources:
  - openapi/karmacheck-api-openapi.yml
  type: http
slug: karmacheck-authentication
source_filename: karmacheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: openapi/karmacheck-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/karmacheck-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/authentication/karmacheck-authentication.yml
summary_line: http · 1 scheme
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Credential Verification
- Motor Vehicle Records
- Occupational Health Screening
- Drug Screening
- HR Tech
- Staffing
- Healthcare
- Compliance
- FCRA
- Adjudication
- Webhook
- MCP Server
- agent-native
---
