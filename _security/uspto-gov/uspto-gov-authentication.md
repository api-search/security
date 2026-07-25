---
api_key_in:
- header
api_specs:
- filename: uspto-gov-appeals-api-openapi.yml
  format: yaml
  label: USPTO Appeals API
  slug: uspto-gov-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-appeals-api-openapi.yml
- filename: uspto-gov-application-api-openapi.yml
  format: yaml
  label: USPTO Application API
  slug: uspto-gov-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-application-api-openapi.yml
- filename: uspto-gov-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-gov-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-assignments-api-openapi.yml
- filename: uspto-gov-citations-api-openapi.yml
  format: yaml
  label: USPTO Citations API
  slug: uspto-gov-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-citations-api-openapi.yml
- filename: uspto-gov-datasets-api-openapi.yml
  format: yaml
  label: USPTO Datasets API
  slug: uspto-gov-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-datasets-api-openapi.yml
- filename: uspto-gov-decisions-api-openapi.yml
  format: yaml
  label: USPTO Decisions API
  slug: uspto-gov-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-decisions-api-openapi.yml
- filename: uspto-gov-documents-api-openapi.yml
  format: yaml
  label: USPTO Documents API
  slug: uspto-gov-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-documents-api-openapi.yml
- filename: uspto-gov-enriched-citations-api-openapi.yml
  format: yaml
  label: USPTO Enriched Citations API
  slug: uspto-gov-enriched-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-enriched-citations-api-openapi.yml
- filename: uspto-gov-office-actions-api-openapi.yml
  format: yaml
  label: USPTO Office Actions API
  slug: uspto-gov-office-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-office-actions-api-openapi.yml
- filename: uspto-gov-patentsview-api-openapi.yml
  format: yaml
  label: USPTO Patentsview API
  slug: uspto-gov-patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-patentsview-api-openapi.yml
- filename: uspto-gov-proceedings-api-openapi.yml
  format: yaml
  label: USPTO Proceedings API
  slug: uspto-gov-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-proceedings-api-openapi.yml
- filename: uspto-gov-rejections-api-openapi.yml
  format: yaml
  label: USPTO Rejections API
  slug: uspto-gov-rejections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-rejections-api-openapi.yml
- filename: uspto-gov-search-api-openapi.yml
  format: yaml
  label: USPTO Search API
  slug: uspto-gov-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-search-api-openapi.yml
- filename: uspto-gov-status-api-openapi.yml
  format: yaml
  label: USPTO Status API
  slug: uspto-gov-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uspto Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: USPTO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: USPTO
provider_slug: uspto-gov
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/uspto-bulk-data-openapi.yml
  - openapi/uspto-office-actions-openapi.yml
  - openapi/uspto-patent-file-wrapper-openapi.yml
  - openapi/uspto-patentsview-openapi.yml
  - openapi/uspto-ptab-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: USPTO-API-KEY
  sources:
  - openapi/uspto-tsdr-openapi.yml
  type: apiKey
slug: uspto-gov-authentication
source_filename: uspto-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uspto-bulk-data-openapi.yml, openapi/uspto-office-actions-openapi.yml, openapi/uspto-patent-file-wrapper-openapi.yml,\n  openapi/uspto-patentsview-openapi.yml, openapi/uspto-ptab-openapi.yml, openapi/uspto-tsdr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/uspto-bulk-data-openapi.yml\n  - openapi/uspto-office-actions-openapi.yml\n  - openapi/uspto-patent-file-wrapper-openapi.yml\n  - openapi/uspto-patentsview-openapi.yml\n  - openapi/uspto-ptab-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: USPTO-API-KEY\n  sources:\n  - openapi/uspto-tsdr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/authentication/uspto-gov-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Patents
- Trademarks
- Intellectual Property
- Government
- Federal
- Open Data
- PTAB
- TSDR
---
