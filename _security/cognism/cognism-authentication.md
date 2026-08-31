---
api_key_in:
- query
api_specs:
- filename: cognism-compliance-api-openapi.yml
  format: yaml
  label: Cognism Compliance API
  slug: cognism-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-compliance-api-openapi.yml
- filename: cognism-enrich-api-openapi.yml
  format: yaml
  label: Cognism Enrich API
  slug: cognism-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-enrich-api-openapi.yml
- filename: cognism-entitlement-api-openapi.yml
  format: yaml
  label: Cognism Entitlement API
  slug: cognism-entitlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-entitlement-api-openapi.yml
- filename: cognism-filter-api-openapi.yml
  format: yaml
  label: Cognism Filter API
  slug: cognism-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-filter-api-openapi.yml
- filename: cognism-redeem-api-openapi.yml
  format: yaml
  label: Cognism Redeem API
  slug: cognism-redeem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-redeem-api-openapi.yml
- filename: cognism-search-api-openapi.yml
  format: yaml
  label: Cognism Search API
  slug: cognism-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cognism Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognism secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cognism
provider_slug: cognism
scheme_count: 2
schemes:
- description: 'API token issued in the Cognism app under Settings > Tokens and API. Sent as `Authorization: Bearer <token>`. Tokens have a time-to-live of 6 months.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cognism-api-openapi.yml
  type: http
- description: Alternative to the Authorization header. Cognism documents it but recommends the header instead, as the query string is less secure.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/cognism-api-openapi.yml
  type: apiKey
slug: cognism-authentication
source_filename: cognism-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/cognism-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued in the Cognism app under Settings > Tokens and API. Sent as\n    `Authorization: Bearer <token>`. Tokens have a time-to-live of 6 months.'\n  sources:\n  - openapi/cognism-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Alternative to the Authorization header. Cognism documents it but recommends\n    the header instead, as the query string is less secure.\n  sources:\n  - openapi/cognism-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/authentication/cognism-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- GDPR
- Intent Data
- Lead Generation
- Firmographics
- Technographics
- Company Data
- Prospecting
- Data as a Service
---
