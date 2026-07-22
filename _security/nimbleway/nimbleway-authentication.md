---
api_key_in: []
api_specs:
- filename: nimbleway-openapi.json
  format: json
  label: Nimble SDK
  slug: nimble-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nimbleway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nimbleway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nimbleway
provider_slug: nimbleway
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nimbleway-openapi.json
  type: http
slug: nimbleway-authentication
source_filename: nimbleway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nimbleway-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nimbleway-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/authentication/nimbleway-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web Data
- Web Scraping
- Data Extraction
- Web Search
- Proxies
- AI Agents
- Model Context Protocol
---
