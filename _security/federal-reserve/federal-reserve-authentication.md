---
api_key_in:
- query
api_specs:
- filename: federal-reserve-category-api-openapi.yml
  format: yaml
  label: Federal Reserve Category API
  slug: federal-reserve-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-category-api-openapi.yml
- filename: federal-reserve-related-tags-api-openapi.yml
  format: yaml
  label: Federal Reserve Related Tags API
  slug: federal-reserve-related-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-related-tags-api-openapi.yml
- filename: federal-reserve-release-api-openapi.yml
  format: yaml
  label: Federal Reserve Release API
  slug: federal-reserve-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-release-api-openapi.yml
- filename: federal-reserve-releases-api-openapi.yml
  format: yaml
  label: Federal Reserve Releases API
  slug: federal-reserve-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-releases-api-openapi.yml
- filename: federal-reserve-series-api-openapi.yml
  format: yaml
  label: Federal Reserve Series API
  slug: federal-reserve-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-series-api-openapi.yml
- filename: federal-reserve-source-api-openapi.yml
  format: yaml
  label: Federal Reserve Source API
  slug: federal-reserve-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-source-api-openapi.yml
- filename: federal-reserve-sources-api-openapi.yml
  format: yaml
  label: Federal Reserve Sources API
  slug: federal-reserve-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-sources-api-openapi.yml
- filename: federal-reserve-tags-api-openapi.yml
  format: yaml
  label: Federal Reserve Tags API
  slug: federal-reserve-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Federal Reserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Reserve secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Reserve
provider_slug: federal-reserve
scheme_count: 1
schemes:
- in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/federal-reserve-fred-openapi.yml
  type: apiKey
slug: federal-reserve-authentication
source_filename: federal-reserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/federal-reserve-fred-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/federal-reserve-fred-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/authentication/federal-reserve-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Economics
- Federal-Government
- Finance
---
