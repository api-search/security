---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nomas-fyi-agent-tools-api-openapi.yml
  format: yaml
  label: Nomas Agent Tools API
  slug: nomas-fyi-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-agent-tools-api-openapi.yml
- filename: nomas-fyi-auth-api-openapi.yml
  format: yaml
  label: Nomas Auth API
  slug: nomas-fyi-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-auth-api-openapi.yml
- filename: nomas-fyi-company-facts-api-openapi.yml
  format: yaml
  label: Nomas Company Facts API
  slug: nomas-fyi-company-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-company-facts-api-openapi.yml
- filename: nomas-fyi-dataview-api-openapi.yml
  format: yaml
  label: Nomas Dataview API
  slug: nomas-fyi-dataview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-dataview-api-openapi.yml
- filename: nomas-fyi-export-api-openapi.yml
  format: yaml
  label: Nomas Export API
  slug: nomas-fyi-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-export-api-openapi.yml
- filename: nomas-fyi-failure-to-deliver-ftd-api-openapi.yml
  format: yaml
  label: Nomas Failure to Deliver (FTD) API
  slug: nomas-fyi-failure-to-deliver-ftd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-failure-to-deliver-ftd-api-openapi.yml
- filename: nomas-fyi-filing-filters-api-openapi.yml
  format: yaml
  label: Nomas Filing filters API
  slug: nomas-fyi-filing-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-filing-filters-api-openapi.yml
- filename: nomas-fyi-filings-api-openapi.yml
  format: yaml
  label: Nomas Filings API
  slug: nomas-fyi-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-filings-api-openapi.yml
- filename: nomas-fyi-form-13f-by-institution-api-openapi.yml
  format: yaml
  label: Nomas Form 13F — By Institution API
  slug: nomas-fyi-form-13f-by-institution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-form-13f-by-institution-api-openapi.yml
- filename: nomas-fyi-form-13f-by-security-api-openapi.yml
  format: yaml
  label: Nomas Form 13F — By Security API
  slug: nomas-fyi-form-13f-by-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-form-13f-by-security-api-openapi.yml
- filename: nomas-fyi-insider-trading-api-openapi.yml
  format: yaml
  label: Nomas Insider Trading API
  slug: nomas-fyi-insider-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-insider-trading-api-openapi.yml
- filename: nomas-fyi-internal-api-openapi.yml
  format: yaml
  label: Nomas Internal API
  slug: nomas-fyi-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-internal-api-openapi.yml
- filename: nomas-fyi-payments-api-openapi.yml
  format: yaml
  label: Nomas Payments API
  slug: nomas-fyi-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-payments-api-openapi.yml
- filename: nomas-fyi-rag-api-openapi.yml
  format: yaml
  label: Nomas RAG API
  slug: nomas-fyi-rag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-rag-api-openapi.yml
- filename: nomas-fyi-realtime-sec-api-openapi.yml
  format: yaml
  label: Nomas Realtime SEC API
  slug: nomas-fyi-realtime-sec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-realtime-sec-api-openapi.yml
- filename: nomas-fyi-schema-api-openapi.yml
  format: yaml
  label: Nomas Schema API
  slug: nomas-fyi-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-schema-api-openapi.yml
- filename: nomas-fyi-user-security-watchlist-api-openapi.yml
  format: yaml
  label: Nomas User Security Watchlist API
  slug: nomas-fyi-user-security-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomas-fyi/openapi/nomas-fyi-user-security-watchlist-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Nomas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nomas secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nomas
provider_slug: nomas-fyi
scheme_count: 3
schemes:
- description: API key from Account Management
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/nomas-fyi-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/nomas-fyi-openapi.yml
  type: http
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/nomas-fyi-openapi.yml
  type: apiKey
slug: nomas-fyi-authentication
source_filename: nomas-fyi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nomas-fyi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key from Account Management\n  sources:\n  - openapi/nomas-fyi-openapi.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nomas-fyi-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/nomas-fyi-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nomas-fyi/authentication/nomas-fyi-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Finance
- Data
- SEC
- Agents
---
