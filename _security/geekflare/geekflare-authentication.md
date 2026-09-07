---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: geekflare-openapi.json
  format: json
  label: Geekflare API
  slug: geekflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geekflare/refs/heads/main/openapi/geekflare-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Geekflare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geekflare secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Geekflare
provider_slug: geekflare
scheme_count: 4
schemes:
- description: API Key required for all endpoints
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/geekflare-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: JWT token for Admin endpoints
  name: bearer-token
  scheme: bearer
  sources:
  - openapi/geekflare-openapi.json
  type: http
- description: IDP session cookie
  in: cookie
  name: gf_auth_session
  parameter: gf_auth_session
  sources:
  - openapi/geekflare-openapi.json
  type: apiKey
- description: Internal API key (Swagger only)
  in: header
  name: x-internal-key
  parameter: x-internal-key
  sources:
  - openapi/geekflare-openapi.json
  type: apiKey
slug: geekflare-authentication
source_filename: geekflare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/geekflare-openapi.json + https://docs.geekflare.com/intro\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key required for all endpoints\n  sources:\n  - openapi/geekflare-openapi.json\n- name: bearer-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for Admin endpoints\n  sources:\n  - openapi/geekflare-openapi.json\n- name: gf_auth_session\n  type: apiKey\n  in: cookie\n  parameter: gf_auth_session\n  description: IDP session cookie\n  sources:\n  - openapi/geekflare-openapi.json\n- name: x-internal-key\n  type: apiKey\n  in: header\n  parameter: x-internal-key\n  description: Internal API key (Swagger only)\n  sources:\n  - openapi/geekflare-openapi.json\ndocs: https://docs.geekflare.com/intro\nnote: 'Public API consumers authenticate with the x-api-key\
  \ header only — one key across every endpoint, single shared credit\n  pool, obtained free at auth.geekflare.com/register. The bearer-token (JWT, admin), gf_auth_session (IDP cookie) and x-internal-key\n  schemes declared in the spec are internal/dashboard surfaces, not for API customers. 401 bodies: \"Missing x-api-key header\"\n  / \"Invalid x-api-key\".'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geekflare/refs/heads/main/authentication/geekflare-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Development
- Public APIs
- Web Scraping
- Search
- Screenshots
- DNS
- Website Monitoring
- Security Testing
- AI Agents
- MCP
---
