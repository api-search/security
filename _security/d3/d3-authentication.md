---
api_key_in:
- header
api_specs:
- filename: d3-doma-openapi.json
  format: json
  label: Doma Protocol API
  slug: doma-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d3/refs/heads/main/openapi/d3-doma-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: D3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: D3 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: D3
provider_slug: d3
scheme_count: 1
schemes:
- in: header
  name: Api-Key
  parameter: Api-Key
  sources:
  - openapi/d3-doma-openapi.json
  type: apiKey
slug: d3-authentication
source_filename: d3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/d3-doma-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  sources:\n  - openapi/d3-doma-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d3/refs/heads/main/authentication/d3-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto Infrastructure
- Domains
- DNS
- Blockchain
- Tokenization
- Web3
- DomainFi
- Marketplace
- Agentic Commerce
---
