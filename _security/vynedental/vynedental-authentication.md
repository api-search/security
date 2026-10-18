---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vynedental-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility and Benefits API (Onederful)
  slug: eligibility-and-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-api-openapi.yml
- filename: vynedental-async-api-openapi.yml
  format: yaml
  label: Vyne Dental Async API
  slug: vynedental-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-async-api-openapi.yml
- filename: vynedental-edi-api-openapi.yml
  format: yaml
  label: Vyne Dental EDI API
  slug: vynedental-edi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-edi-api-openapi.yml
- filename: vynedental-eligibility-response-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Response API
  slug: vynedental-eligibility-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-response-api-openapi.yml
- filename: vynedental-eligibility-status-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Status API
  slug: vynedental-eligibility-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-status-api-openapi.yml
- filename: vynedental-enhanced-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Enhanced Eligibility API
  slug: vynedental-enhanced-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-enhanced-eligibility-api-openapi.yml
- filename: vynedental-oauth2-api-openapi.yml
  format: yaml
  label: Vyne Dental Oauth2 API
  slug: vynedental-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-oauth2-api-openapi.yml
- filename: vynedental-well-known-api-openapi.yml
  format: yaml
  label: Vyne Dental .well Known API
  slug: vynedental-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vynedental Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vyne Dental declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vyne Dental
provider_slug: vynedental
scheme_count: 1
schemes:
- flow: client_credentials
  header: 'Authorization: Bearer <token>'
  scopes:
  - feature:eligibility
  token_format: JWT
  token_lifetime_seconds: 3600
  token_url: https://production.onederful.co/oauth2/token
  type: oauth2
slug: vynedental-authentication
source_filename: vynedental-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://developers.onederful.co/documentation/\nsummary: Every Vyne API request carries a JWT bearer token obtained by POSTing client_id and client_secret (JSON body) to https://production.onederful.co/oauth2/token; tokens return scope feature:eligibility, expires_in 3600, token_type Bearer. A token invalidation endpoint (/oauth2/token/invalidate) and a JWKS (/.well-known/jwks.json) are published in the OpenAPI.\nschemes:\n- type: oauth2\n  flow: client_credentials\n  token_url: https://production.onederful.co/oauth2/token\n  token_format: JWT\n  scopes:\n  - feature:eligibility\n  header: 'Authorization: Bearer <token>'\n  token_lifetime_seconds: 3600\ndocs: https://developers.onederful.co/documentation/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/authentication/vynedental-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Dental
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- Payments
---
