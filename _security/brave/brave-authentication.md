---
api_key_in:
- header
api_specs:
- filename: brave-search-api.yml
  format: yaml
  label: Brave Search API
  slug: brave-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-search-api.yml
- filename: brave-ads-api.yml
  format: yaml
  label: Brave Ads API
  slug: brave-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-ads-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brave secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Brave
provider_slug: brave
scheme_count: 2
schemes:
- description: API key generated from the Brave Ads dashboard at https://ads.brave.com.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/brave-ads-api.yml
  type: apiKey
- description: API key obtained from the Brave Search API dashboard at https://api-dashboard.search.brave.com
  in: header
  name: ApiKeyAuth
  parameter: X-Subscription-Token
  sources:
  - openapi/brave-search-api.yml
  type: apiKey
slug: brave-authentication
source_filename: brave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brave-ads-api.yml, openapi/brave-search-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key generated from the Brave Ads dashboard at https://ads.brave.com.\n  sources:\n  - openapi/brave-ads-api.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Subscription-Token\n  description: API key obtained from the Brave Search API dashboard at https://api-dashboard.search.brave.com\n  sources:\n  - openapi/brave-search-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/authentication/brave-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Search
- Advertising
- Privacy
- Browser
- AI
- LLM
---
