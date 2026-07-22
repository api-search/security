---
api_key_in:
- header
api_specs:
- filename: r2-openapi.json
  format: json
  label: R2 API
  slug: r2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r2/refs/heads/main/openapi/r2-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: R2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: R2 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: R2
provider_slug: r2
scheme_count: 1
schemes:
- claims:
  - kid (header) — keyId issued by R2
  - mid — merchant id (optional for API, required for embeddable components)
  - country — ISO-2 country code (optional; needed for multi-country partners)
  - exp — expiry (seconds)
  environments:
  - dev
  - prod
  in: header
  name: JWT
  parameter: Authorization
  signing_algorithm: HS256
  sources:
  - openapi/r2-openapi.json
  - https://r2-api-docs.readme.io/docs/jwt-token-generation
  token_format: JWT
  type: apiKey
slug: r2-authentication
source_filename: r2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/r2-openapi.json\ndocs: https://r2-api-docs.readme.io/docs/jwt-token-generation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  R2 authorizes API calls with a short-lived JWT bearer token supplied in the\n  Authorization header. Partners request access by emailing partners@r2.co and\n  receive two credential sets (keyId + JWTSecret) for the dev and prod\n  environments. The partner signs its own JWTs with HS256 (HMAC-SHA256), setting\n  the keyId as the token `kid` header plus optional `mid` (merchant id) and\n  `country` (ISO-2) claims and an `exp` expiry. Merchant id is required when\n  initializing embeddable components.\nschemes:\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  token_format: JWT\n  signing_algorithm: HS256\n  claims:\n  - kid (header) — keyId issued by R2\n  - mid — merchant id (optional for API, required for embeddable components)\n  - country —\
  \ ISO-2 country code (optional; needed for multi-country partners)\n  - exp — expiry (seconds)\n  environments:\n  - dev\n  - prod\n  sources:\n  - openapi/r2-openapi.json\n  - https://r2-api-docs.readme.io/docs/jwt-token-generation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r2/refs/heads/main/authentication/r2-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Financial Services
- Embedded Finance
- Lending
- Payments
- Fintech
- Latin America
- Revenue-Based Financing
- Webhooks
---
