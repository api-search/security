---
api_key_in:
- header
- query
api_specs:
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: domain-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: email-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: email-verifier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: email-count
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: discover
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: email-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: company-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: combined-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: leads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: leads-lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Logo API
  slug: logo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
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
