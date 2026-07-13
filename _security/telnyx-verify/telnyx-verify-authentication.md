---
api_key_in: []
api_specs:
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Verifications API
  slug: telnyx-verify-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Profiles API
  slug: telnyx-verify-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Number Lookup API
  slug: telnyx-verify-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Telnyx Verify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telnyx Verify API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telnyx Verify API
provider_slug: telnyx-verify
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'Telnyx API v2 key passed as `Authorization: Bearer YOUR_API_KEY`. Create and manage keys in the Telnyx Mission Control Portal under Auth / API Keys (portal.telnyx.com). The same key authenticates Verify, Verify Profiles, and Number Lookup as well as the rest of the Telnyx API v2 surface.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/telnyx-verify-openapi.yml
  type: http
slug: telnyx-verify-authentication
source_filename: telnyx-verify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telnyx-verify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Telnyx API v2 key passed as `Authorization: Bearer YOUR_API_KEY`. Create\n    and manage keys in the Telnyx Mission Control Portal under Auth / API Keys\n    (portal.telnyx.com). The same key authenticates Verify, Verify Profiles, and\n    Number Lookup as well as the rest of the Telnyx API v2 surface.'\n  sources:\n  - openapi/telnyx-verify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/authentication/telnyx-verify-authentication.yml
summary_line: http · 1 scheme
tags:
- Number Verification
- Phone Verification
- OTP
- 2FA
- Lookup
- Verify
- Number Lookup
- CNAM
- Identity
- Anti-Fraud
---
