---
api_key_in:
- header
api_specs:
- filename: unify-data-openapi.json
  format: json
  label: Unify Data API
  slug: unify-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-data-openapi.json
- filename: unify-sequences-openapi.json
  format: json
  label: Unify Sequences API
  slug: unify-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequences-openapi.json
- filename: unify-analytics-openapi.json
  format: json
  label: Unify Analytics API
  slug: unify-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-analytics-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Unify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unify secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unify
provider_slug: unify
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: Basic
  sources:
  - openapi/unify-analytics-openapi.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/unify-data-openapi.json
  - openapi/unify-sequences-openapi.json
  type: apiKey
slug: unify-authentication
source_filename: unify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unify-analytics-openapi.json, openapi/unify-data-openapi.json, openapi/unify-sequences-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: Basic\n  sources:\n  - openapi/unify-analytics-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/unify-data-openapi.json\n  - openapi/unify-sequences-openapi.json\ndocs: https://docs.unifygtm.com/developers/introduction\nnotes: API keys are generated in the Unify app under Settings -> Developers (app.unifygtm.com/dashboard/settings/integrations/api-keys)\n  and sent in the x-api-key header on the Data and Sequences APIs. The Bulk API requires a user-backed\n  API key. The Analytics API authenticates with HTTP Basic using a public write key suitable\n  for client-side event collection.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/authentication/unify-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Sales
- Marketing
- Go-To-Market
- Outbound
- Intent Data
- AI Agents
- B2B
- Data Enrichment
- Sequences
- Analytics
---
