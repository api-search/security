---
api_key_in:
- header
api_specs:
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Sessions API
  slug: veriff-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Decisions API
  slug: veriff-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Person API
  slug: veriff-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Media API
  slug: veriff-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Watchlist Screening API
  slug: veriff-watchlist-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Attempts API
  slug: veriff-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Webhooks API
  slug: veriff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veriff Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veriff secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Veriff
provider_slug: veriff-com
scheme_count: 2
schemes:
- description: Your integration's public API key.
  in: header
  name: AuthClient
  parameter: X-AUTH-CLIENT
  sources:
  - openapi/veriff-com-openapi.yml
  type: apiKey
- description: Hex-encoded HMAC-SHA256 signature of the payload (POST/PATCH) or the resource ID (GET/DELETE), keyed with your integration's shared secret.
  in: header
  name: HmacSignature
  parameter: X-HMAC-SIGNATURE
  sources:
  - openapi/veriff-com-openapi.yml
  type: apiKey
slug: veriff-com-authentication
source_filename: veriff-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veriff-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthClient\n  type: apiKey\n  in: header\n  parameter: X-AUTH-CLIENT\n  description: Your integration's public API key.\n  sources:\n  - openapi/veriff-com-openapi.yml\n- name: HmacSignature\n  type: apiKey\n  in: header\n  parameter: X-HMAC-SIGNATURE\n  description: Hex-encoded HMAC-SHA256 signature of the payload (POST/PATCH) or the resource\n    ID (GET/DELETE), keyed with your integration's shared secret.\n  sources:\n  - openapi/veriff-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/authentication/veriff-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Identity Verification
- KYC
- AML
- Biometrics
- Document Verification
- Fraud Prevention
---
