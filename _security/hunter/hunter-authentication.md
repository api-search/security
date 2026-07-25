---
api_key_in:
- header
- query
api_specs:
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-campaigns-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: hunter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-campaigns-api-openapi.yml
- filename: hunter-combined-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: hunter-combined-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-combined-enrichment-api-openapi.yml
- filename: hunter-company-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: hunter-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-company-enrichment-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-email-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: hunter-email-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-enrichment-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-api-openapi.yml
- filename: hunter-leads-lists-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: hunter-leads-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-lists-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hunter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hunter secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hunter
provider_slug: hunter
scheme_count: 3
schemes:
- description: API key passed as a query parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/hunter-api-openapi.yml
  type: apiKey
- description: API key passed via the X-API-KEY header.
  in: header
  name: apiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/hunter-api-openapi.yml
  type: apiKey
- description: API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hunter-api-openapi.yml
  type: http
slug: hunter-authentication
source_filename: hunter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hunter-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter.\n  sources:\n  - openapi/hunter-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key passed via the X-API-KEY header.\n  sources:\n  - openapi/hunter-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/hunter-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/authentication/hunter-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
---
