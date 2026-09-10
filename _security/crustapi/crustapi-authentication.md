---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: CrustAPI
  slug: crustapi
  spec_type: OpenAPI
  url: https://crustapi.com/v1/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crustapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrustAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CrustAPI
provider_slug: crustapi
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/crustapi-openapi.json
  type: apiKey
slug: crustapi-authentication
source_filename: crustapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: openapi/crustapi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/crustapi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crustapi/refs/heads/main/authentication/crustapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- Google Maps
- LinkedIn
- SERP / Web Scraping
- Business & Lead Data
- People / Recruiting Data
- Data Enrichment
- AI Agents / MCP
- RAG
- Data
---
