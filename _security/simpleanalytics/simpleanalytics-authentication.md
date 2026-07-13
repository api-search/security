---
api_key_in:
- header
api_specs:
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Stats API
  slug: simpleanalytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Export API
  slug: simpleanalytics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Events API
  slug: simpleanalytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Websites API
  slug: simpleanalytics-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Simpleanalytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simple Analytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Simple Analytics
provider_slug: simpleanalytics
scheme_count: 2
schemes:
- description: API key starting with sa_api_key_
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/simpleanalytics-openapi.yml
  type: apiKey
- description: User identifier starting with sa_user_id_
  in: header
  name: UserId
  parameter: User-Id
  sources:
  - openapi/simpleanalytics-openapi.yml
  type: apiKey
slug: simpleanalytics-authentication
source_filename: simpleanalytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simpleanalytics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API key starting with sa_api_key_\n  sources:\n  - openapi/simpleanalytics-openapi.yml\n- name: UserId\n  type: apiKey\n  in: header\n  parameter: User-Id\n  description: User identifier starting with sa_user_id_\n  sources:\n  - openapi/simpleanalytics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/authentication/simpleanalytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
---
