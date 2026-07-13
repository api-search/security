---
api_key_in: []
api_specs:
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Verification API
  slug: prelude-so-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Lookup API
  slug: prelude-so-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Watch Anti-Fraud API
  slug: prelude-so-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Transactional Messaging API
  slug: prelude-so-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prelude So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prelude secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prelude
provider_slug: prelude-so
scheme_count: 1
schemes:
- description: 'Bearer API key passed as `Authorization: Bearer YOUR_API_KEY`. Keys are issued from the Prelude dashboard under All Services > Configure > Keys. In API v2 this replaced the v1 `X-API-Key` header and the previously required `CUSTOMER_UUID` header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prelude-so-openapi.yml
  - https://docs.prelude.so/verify/v2/documentation/v2-migration-guide
  type: http
slug: prelude-so-authentication
source_filename: prelude-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prelude-so-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API key passed as `Authorization: Bearer YOUR_API_KEY`. Keys are\n    issued from the Prelude dashboard under All Services > Configure > Keys. In\n    API v2 this replaced the v1 `X-API-Key` header and the previously required\n    `CUSTOMER_UUID` header.\n  sources:\n  - openapi/prelude-so-openapi.yml\n  - https://docs.prelude.so/verify/v2/documentation/v2-migration-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/authentication/prelude-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Number Verification
- Phone Verification
- OTP
- Authentication
- Anti-Fraud
- Two-Factor Authentication
- SMS
- Phone Number Lookup
---
