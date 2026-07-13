---
api_key_in:
- header
api_specs:
- filename: socure-idplus-api-openapi.yml
  format: yaml
  label: Socure ID+ API
  slug: socure-idplus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-idplus-api-openapi.yml
- filename: socure-docv-api-openapi.yml
  format: yaml
  label: Socure Predictive DocV API
  slug: socure-docv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-docv-api-openapi.yml
- filename: socure-watchlist-monitoring-api-openapi.yml
  format: yaml
  label: Socure Global Watchlist Monitoring API
  slug: socure-watchlist-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-watchlist-monitoring-api-openapi.yml
- filename: socure-decision-api-openapi.yml
  format: yaml
  label: Socure Decision API
  slug: socure-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-decision-api-openapi.yml
- filename: socure-account-intelligence-api-openapi.yml
  format: yaml
  label: Socure Account Intelligence API
  slug: socure-account-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-account-intelligence-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Socure Authentication
name_suffix: Authentication
oauth_flows: []
overview: socure secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: socure
provider_slug: socure
scheme_count: 1
schemes:
- in: header
  name: SocureToken
  parameter: Authorization
  sources:
  - openapi/socure-account-intelligence-api-openapi.yml
  - openapi/socure-decision-api-openapi.yml
  - openapi/socure-docv-api-openapi.yml
  - openapi/socure-idplus-api-openapi.yml
  - openapi/socure-watchlist-monitoring-api-openapi.yml
  type: apiKey
slug: socure-authentication
source_filename: socure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/socure-account-intelligence-api-openapi.yml, openapi/socure-decision-api-openapi.yml,\n  openapi/socure-docv-api-openapi.yml, openapi/socure-idplus-api-openapi.yml, openapi/socure-watchlist-monitoring-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SocureToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/socure-account-intelligence-api-openapi.yml\n  - openapi/socure-decision-api-openapi.yml\n  - openapi/socure-docv-api-openapi.yml\n  - openapi/socure-idplus-api-openapi.yml\n  - openapi/socure-watchlist-monitoring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/authentication/socure-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
