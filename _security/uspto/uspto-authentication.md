---
api_key_in:
- header
api_specs:
- filename: uspto-patent-api-openapi.yml
  format: yaml
  label: USPTO Patent & Trademark API
  slug: patent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-patent-api-openapi.yml
- filename: index.html
  format: yaml
  label: USPTO Patent Trial and Appeal Board (PTAB) API
  slug: ptab-api
  spec_type: OpenAPI
  url: https://data.uspto.gov/swagger/index.html
- filename: tsdr-api-v1
  format: yaml
  label: USPTO Trademark Status and Document Retrieval (TSDR) API
  slug: tsdr-api
  spec_type: OpenAPI
  url: https://developer.uspto.gov/swagger/tsdr-api-v1
- filename: oa_actions.json
  format: json
  label: USPTO Office Action Text Retrieval API
  slug: office-actions-api
  spec_type: OpenAPI
  url: https://developer.uspto.gov/ds-api/swagger/docs/oa_actions.json
- filename: enriched_cited_reference_metadata.json
  format: json
  label: USPTO Enriched Citation API
  slug: enriched-citation-api
  spec_type: OpenAPI
  url: https://developer.uspto.gov/ds-api/swagger/docs/enriched_cited_reference_metadata.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uspto Authentication
name_suffix: Authentication
oauth_flows: []
overview: USPTO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: USPTO
provider_slug: uspto
scheme_count: 1
schemes:
- description: USPTO Open Data Portal API key
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/uspto-patent-api-openapi.yml
  type: apiKey
slug: uspto-authentication
source_filename: uspto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uspto-patent-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: USPTO Open Data Portal API key\n  sources:\n  - openapi/uspto-patent-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/authentication/uspto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Intellectual Property
- Open Data
- Patents
- Regulatory
- Trademarks
- USPTO
---
