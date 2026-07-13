---
api_key_in: []
api_specs:
- filename: aligned-news-openapi.yml
  format: yaml
  label: Aligned News
  slug: aligned-news
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-openapi.yml
- filename: aligned-news-openapi.yml
  format: yaml
  label: Aligned News REST API
  slug: aligned-news-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aligned News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aligned News secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aligned News
provider_slug: aligned-news
scheme_count: 1
schemes:
- bearerFormat: alnw_*
  description: API key issued from https://alignednews.com/account, presented as Authorization Bearer alnw_...
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aligned-news-openapi.yml
  type: http
slug: aligned-news-authentication
source_filename: aligned-news-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aligned-news-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: alnw_*\n  description: API key issued from https://alignednews.com/account, presented as Authorization\n    Bearer alnw_...\n  sources:\n  - openapi/aligned-news-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/authentication/aligned-news-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- News
- Intelligence
- MCP
- Signals
---
