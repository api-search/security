---
api_key_in:
- header
- query
api_specs:
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Enrichment API
  slug: hunter-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-enrichment-api-openapi.yml
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-leads-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hunter Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hunter secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hunter
provider_slug: hunter-io
scheme_count: 3
schemes:
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/hunter-account-api-openapi.yml
  - openapi/hunter-discover-api-openapi.yml
  - openapi/hunter-domain-search-api-openapi.yml
  - openapi/hunter-email-finder-api-openapi.yml
  - openapi/hunter-email-verifier-api-openapi.yml
  - openapi/hunter-enrichment-api-openapi.yml
  - openapi/hunter-leads-api-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/hunter-account-api-openapi.yml
  - openapi/hunter-discover-api-openapi.yml
  - openapi/hunter-domain-search-api-openapi.yml
  - openapi/hunter-email-finder-api-openapi.yml
  - openapi/hunter-email-verifier-api-openapi.yml
  - openapi/hunter-enrichment-api-openapi.yml
  - openapi/hunter-leads-api-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hunter-account-api-openapi.yml
  - openapi/hunter-discover-api-openapi.yml
  - openapi/hunter-domain-search-api-openapi.yml
  - openapi/hunter-email-finder-api-openapi.yml
  - openapi/hunter-email-verifier-api-openapi.yml
  - openapi/hunter-enrichment-api-openapi.yml
  - openapi/hunter-leads-api-openapi.yml
  type: http
slug: hunter-io-authentication
source_filename: hunter-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hunter-account-api-openapi.yml, openapi/hunter-discover-api-openapi.yml, openapi/hunter-domain-search-api-openapi.yml,\n  openapi/hunter-email-finder-api-openapi.yml, openapi/hunter-email-verifier-api-openapi.yml,\n  openapi/hunter-enrichment-api-openapi.yml, openapi/hunter-leads-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/hunter-account-api-openapi.yml\n  - openapi/hunter-discover-api-openapi.yml\n  - openapi/hunter-domain-search-api-openapi.yml\n  - openapi/hunter-email-finder-api-openapi.yml\n  - openapi/hunter-email-verifier-api-openapi.yml\n  - openapi/hunter-enrichment-api-openapi.yml\n  - openapi/hunter-leads-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/hunter-account-api-openapi.yml\n\
  \  - openapi/hunter-discover-api-openapi.yml\n  - openapi/hunter-domain-search-api-openapi.yml\n  - openapi/hunter-email-finder-api-openapi.yml\n  - openapi/hunter-email-verifier-api-openapi.yml\n  - openapi/hunter-enrichment-api-openapi.yml\n  - openapi/hunter-leads-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hunter-account-api-openapi.yml\n  - openapi/hunter-discover-api-openapi.yml\n  - openapi/hunter-domain-search-api-openapi.yml\n  - openapi/hunter-email-finder-api-openapi.yml\n  - openapi/hunter-email-verifier-api-openapi.yml\n  - openapi/hunter-enrichment-api-openapi.yml\n  - openapi/hunter-leads-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/authentication/hunter-io-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Email Finder
- Email Verifier
- Lead Generation
- Outreach
- Prospecting
- Enrichment
- Sales
- Marketing
---
