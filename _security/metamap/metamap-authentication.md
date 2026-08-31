---
api_key_in: []
api_specs:
- filename: metamap-authentication-api-openapi.yml
  format: yaml
  label: MetaMap Authentication API
  slug: metamap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-authentication-api-openapi.yml
- filename: metamap-background-checks-api-openapi.yml
  format: yaml
  label: MetaMap Background Checks API
  slug: metamap-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-background-checks-api-openapi.yml
- filename: metamap-credit-checks-api-openapi.yml
  format: yaml
  label: MetaMap Credit Checks API
  slug: metamap-credit-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-credit-checks-api-openapi.yml
- filename: metamap-custom-watchlists-api-openapi.yml
  format: yaml
  label: MetaMap Custom Watchlists API
  slug: metamap-custom-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-custom-watchlists-api-openapi.yml
- filename: metamap-email-checks-api-openapi.yml
  format: yaml
  label: MetaMap Email Checks API
  slug: metamap-email-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-email-checks-api-openapi.yml
- filename: metamap-govchecks-api-openapi.yml
  format: yaml
  label: MetaMap GovChecks API
  slug: metamap-govchecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-govchecks-api-openapi.yml
- filename: metamap-phone-checks-api-openapi.yml
  format: yaml
  label: MetaMap Phone Checks API
  slug: metamap-phone-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-phone-checks-api-openapi.yml
- filename: metamap-verifications-api-openapi.yml
  format: yaml
  label: MetaMap Verifications API
  slug: metamap-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-verifications-api-openapi.yml
- filename: metamap-watchlist-checks-api-openapi.yml
  format: yaml
  label: MetaMap Watchlist Checks API
  slug: metamap-watchlist-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-watchlist-checks-api-openapi.yml
- filename: metamap-webhooks-api-openapi.yml
  format: yaml
  label: MetaMap Webhooks API
  slug: metamap-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/openapi/metamap-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Metamap Authentication
name_suffix: Authentication
oauth_flows: []
overview: MetaMap secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MetaMap
provider_slug: metamap
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT obtained via POST /oauth using client_id / client_secret as HTTP Basic.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/metamap-openapi.yml
  type: http
- description: Used only on POST /oauth for the initial token exchange.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/metamap-openapi.yml
  type: http
slug: metamap-authentication
source_filename: metamap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metamap-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT obtained via POST /oauth using client_id / client_secret as HTTP Basic.\n  sources:\n  - openapi/metamap-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Used only on POST /oauth for the initial token exchange.\n  sources:\n  - openapi/metamap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metamap/refs/heads/main/authentication/metamap-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Verification
- KYC
- AML
- Anti-Money Laundering
- Compliance
- Biometrics
- Document Verification
- Facematch
- Liveness
- GovCheck
- Watchlist
- Background Check
- Credit Check
- Risk
- Fraud Prevention
- Onboarding
- LatAm
- Africa
- Mobile SDK
---
