---
api_key_in:
- header
api_specs:
- filename: structify-openapi-original.json
  format: json
  label: Structify API
  slug: structify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/structify/refs/heads/main/openapi/structify-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Structify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Structify secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Structify
provider_slug: structify
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/structify-openapi-original.json
  type: apiKey
- name: session_token
  scheme: bearer
  sources:
  - openapi/structify-openapi-original.json
  type: http
slug: structify-authentication
source_filename: structify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/structify-openapi-original.json\ndocs: https://docs.structify.ai/api-reference/authentication\nenv_var: STRUCTIFY_API_TOKEN\nnotes: >-\n  API key in the `api_key` header, or a Bearer session token (session_token).\n  The SDKs read the key from the STRUCTIFY_API_TOKEN environment variable. Keys\n  are created in the Structify dashboard under Settings -> API Keys.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/structify-openapi-original.json\n- name: session_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/structify-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/structify/refs/heads/main/authentication/structify-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Data
- Web Scraping
- Data Extraction
- Knowledge Graph
- ETL
- Data Enrichment
---
