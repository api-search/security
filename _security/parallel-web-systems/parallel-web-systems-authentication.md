---
api_key_in:
- header
api_specs:
- filename: parallel-web-systems-openapi.json
  format: json
  label: Parallel API
  slug: parallel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Parallel Web Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallel Web Systems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parallel Web Systems
provider_slug: parallel-web-systems
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/parallel-web-systems-openapi.json
  type: apiKey
slug: parallel-web-systems-authentication
source_filename: parallel-web-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/parallel-web-systems-openapi.json + https://docs.parallel.ai\ndocs: https://docs.parallel.ai/getting-started/overview\nkey_issuance:\n  platform: https://platform.parallel.ai\n  device_oauth_metadata: https://platform.parallel.ai/.well-known/oauth-authorization-server\n  detail: >-\n    Data-plane requests authenticate with a per-account API key in the x-api-key header.\n    Keys are minted at platform.parallel.ai; parallel-cli obtains them via an OAuth 2.0\n    device-code flow (issuer platform.parallel.ai, scope key:read, PKCE S256).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/parallel-web-systems-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/authentication/parallel-web-systems-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Web Search
- Deep Research
- Data Enrichment
- Web Monitoring
- AI Agents
- MCP
---
