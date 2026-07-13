---
api_key_in:
- header
- query
api_specs:
- filename: builtwith-domain-openapi.yml
  format: yaml
  label: BuiltWith Domain API
  slug: builtwith-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-openapi.yml
- filename: builtwith-lists-openapi.yml
  format: yaml
  label: BuiltWith Lists API
  slug: builtwith-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-lists-openapi.yml
- filename: builtwith-trends-openapi.yml
  format: yaml
  label: BuiltWith Trends API
  slug: builtwith-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-trends-openapi.yml
- filename: builtwith-change-openapi.yml
  format: yaml
  label: BuiltWith Change API
  slug: builtwith-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-change-openapi.yml
- filename: builtwith-relationships-openapi.yml
  format: yaml
  label: BuiltWith Relationships API
  slug: builtwith-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-relationships-openapi.yml
- filename: builtwith-free-openapi.yml
  format: yaml
  label: BuiltWith Free API
  slug: builtwith-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-openapi.yml
- filename: builtwith-tags-openapi.yml
  format: yaml
  label: BuiltWith Tags API
  slug: builtwith-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tags-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Builtwith Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuiltWith secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BuiltWith
provider_slug: builtwith
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: KEY
  sources:
  - openapi/builtwith-change-openapi.yml
  - openapi/builtwith-domain-openapi.yml
  - openapi/builtwith-free-openapi.yml
  - openapi/builtwith-lists-openapi.yml
  - openapi/builtwith-relationships-openapi.yml
  - openapi/builtwith-tags-openapi.yml
  - openapi/builtwith-trends-openapi.yml
  type: apiKey
- description: 'Format: ''Authorization: API {key}'''
  in: header
  name: apiKeyHeader
  parameter: Authorization
  sources:
  - openapi/builtwith-change-openapi.yml
  - openapi/builtwith-domain-openapi.yml
  - openapi/builtwith-lists-openapi.yml
  - openapi/builtwith-relationships-openapi.yml
  - openapi/builtwith-tags-openapi.yml
  - openapi/builtwith-trends-openapi.yml
  type: apiKey
slug: builtwith-authentication
source_filename: builtwith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/builtwith-change-openapi.yml, openapi/builtwith-domain-openapi.yml, openapi/builtwith-free-openapi.yml,\n  openapi/builtwith-lists-openapi.yml, openapi/builtwith-relationships-openapi.yml, openapi/builtwith-tags-openapi.yml,\n  openapi/builtwith-trends-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: KEY\n  sources:\n  - openapi/builtwith-change-openapi.yml\n  - openapi/builtwith-domain-openapi.yml\n  - openapi/builtwith-free-openapi.yml\n  - openapi/builtwith-lists-openapi.yml\n  - openapi/builtwith-relationships-openapi.yml\n  - openapi/builtwith-tags-openapi.yml\n  - openapi/builtwith-trends-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format: ''Authorization: API {key}'''\n  sources:\n  - openapi/builtwith-change-openapi.yml\n  - openapi/builtwith-domain-openapi.yml\n\
  \  - openapi/builtwith-lists-openapi.yml\n  - openapi/builtwith-relationships-openapi.yml\n  - openapi/builtwith-tags-openapi.yml\n  - openapi/builtwith-trends-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/authentication/builtwith-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Technology Profiling
- Lead Generation
- Web Intelligence
- Technology Detection
- Website Analysis
- Market Research
---
