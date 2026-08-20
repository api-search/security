---
api_key_in:
- header
api_specs:
- filename: national-cancer-institute-download-api-openapi.yml
  format: yaml
  label: National Cancer Institute Download API
  slug: national-cancer-institute-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/openapi/national-cancer-institute-download-api-openapi.yml
- filename: national-cancer-institute-search-api-openapi.yml
  format: yaml
  label: National Cancer Institute Search API
  slug: national-cancer-institute-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/openapi/national-cancer-institute-search-api-openapi.yml
- filename: national-cancer-institute-status-api-openapi.yml
  format: yaml
  label: National Cancer Institute Status API
  slug: national-cancer-institute-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/openapi/national-cancer-institute-status-api-openapi.yml
- filename: national-cancer-institute-submission-api-openapi.yml
  format: yaml
  label: National Cancer Institute Submission API
  slug: national-cancer-institute-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/openapi/national-cancer-institute-submission-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Cancer Institute Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Cancer Institute secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Cancer Institute
provider_slug: national-cancer-institute
scheme_count: 1
schemes:
- in: header
  name: GdcAuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/national-cancer-institute-openapi.yml
  type: apiKey
slug: national-cancer-institute-authentication
source_filename: national-cancer-institute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-cancer-institute-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: GdcAuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/national-cancer-institute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/authentication/national-cancer-institute-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cancer
- Federal-Government
- Health
- Research
---
