---
api_key_in:
- header
api_specs:
- filename: incode-openapi.yml
  format: yaml
  label: Incode Onboarding Sessions API
  slug: incode-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode ID Verification API
  slug: incode-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Face and Liveness API
  slug: incode-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Government Validation API
  slug: incode-government-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Watchlist and AML API
  slug: incode-watchlist-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Results API
  slug: incode-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Webhooks API
  slug: incode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Incode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incode secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Incode
provider_slug: incode
scheme_count: 2
schemes:
- description: Client API key issued by Incode.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/incode-openapi.yml
  type: apiKey
- description: Session token (Onboarding Token) returned by POST /omni/start.
  in: header
  name: SessionToken
  parameter: X-Incode-Hardware-Id
  sources:
  - openapi/incode-openapi.yml
  type: apiKey
slug: incode-authentication
source_filename: incode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/incode-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Client API key issued by Incode.\n  sources:\n  - openapi/incode-openapi.yml\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: X-Incode-Hardware-Id\n  description: Session token (Onboarding Token) returned by POST /omni/start.\n  sources:\n  - openapi/incode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/authentication/incode-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Identity Verification
- Biometrics
- KYC
- Liveness
- Onboarding
---
