---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: KonbiniAPI Main Spec
  slug: main
  spec_type: OpenAPI
  url: https://docs.konbiniapi.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Konbiniapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: KonbiniAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KonbiniAPI
provider_slug: konbiniapi
scheme_count: 1
schemes:
- description: 'Send your API key in the Authorization header as a Bearer token.

    Example: `Authorization: Bearer <your-api-key>`'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/konbiniapi-openapi.yml
  type: http
slug: konbiniapi-authentication
source_filename: konbiniapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/konbiniapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: |-\n    Send your API key in the Authorization header as a Bearer token.\n    Example: `Authorization: Bearer <your-api-key>`\n  sources:\n  - openapi/konbiniapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/authentication/konbiniapi-authentication.yml
summary_line: http · 1 scheme
tags:
- API
- Social Media
- Instagram
- TikTok
- ActivityStreams 2.0
- Scraping
- Data Extraction
- Public Data
- Influencer Marketing
- Social Listening
- Creator Tools
- MCP
- Model Context Protocol
---
