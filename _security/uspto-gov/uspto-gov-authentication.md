---
api_key_in:
- header
api_specs:
- filename: uspto-patent-file-wrapper-openapi.yml
  format: yaml
  label: USPTO Patent File Wrapper API
  slug: uspto-patent-file-wrapper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patent-file-wrapper-openapi.yml
- filename: uspto-ptab-openapi.yml
  format: yaml
  label: USPTO Patent Trial and Appeal Board (PTAB) API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-ptab-openapi.yml
- filename: uspto-tsdr-openapi.yml
  format: yaml
  label: USPTO Trademark Status and Document Retrieval (TSDR) API
  slug: uspto-tsdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-tsdr-openapi.yml
- filename: uspto-office-actions-openapi.yml
  format: yaml
  label: USPTO Office Action APIs
  slug: uspto-office-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-office-actions-openapi.yml
- filename: uspto-bulk-data-openapi.yml
  format: yaml
  label: USPTO Bulk Data Storage System (BDSS) API
  slug: uspto-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-bulk-data-openapi.yml
- filename: uspto-patentsview-openapi.yml
  format: yaml
  label: USPTO PatentsView API
  slug: patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patentsview-openapi.yml
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
