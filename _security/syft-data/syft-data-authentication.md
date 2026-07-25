---
api_key_in: []
api_specs:
- filename: syft-data-export-api-openapi.yml
  format: yaml
  label: Syft Data Export API
  slug: syft-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-export-api-openapi.yml
- filename: syft-data-lookup-api-openapi.yml
  format: yaml
  label: Syft Data Lookup API
  slug: syft-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-lookup-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Syft Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syft Data declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Syft Data
provider_slug: syft-data
scheme_count: 5
schemes:
- format: 'Authorization: Bearer sk_live_...'
  key_prefix: sk_live_
  location: Authorization header
  name: Server Secret Key (Bearer)
  obtain: https://app.syftdata.com/dashboard/settings/snippets
  scheme: bearer
  type: http
  used_by:
  - Lookup API
  - Export API
  - MCP server
- format: 'x-syft-secret-key: sk_live_...'
  in: header
  name: x-syft-secret-key
  type: apiKey
  used_by:
  - Lookup API
  - Export API
- in: body
  name: secretKey
  type: apiKey
  used_by:
  - Lookup API
- location: client SDK init / data attribute
  name: sourceId
  note: Public source identifier used by the browser tracking pixel; not a secret.
  type: apiKey
  used_by:
  - JavaScript tracking SDK
- issuer: https://syft-studio.us.auth0.com/
  name: MCP OAuth (Auth0)
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
  used_by:
  - MCP server (Claude
  - ChatGPT
  - Claude Code)
slug: syft-data-authentication
source_filename: syft-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.syftdata.com/implementation/lookup-api and https://docs.syftdata.com/ai-agents/connect\napi: Syft Data Lookup & Export API\nsummary: >-\n  Server-side REST APIs authenticate with a Server Secret Key (sk_live_ prefix)\n  as a Bearer token or x-syft-secret-key header. The client-side tracking SDK\n  uses a public sourceId. The MCP server supports OAuth (Auth0) or API-key bearer.\nschemes:\n  - type: http\n    scheme: bearer\n    name: Server Secret Key (Bearer)\n    location: Authorization header\n    format: \"Authorization: Bearer sk_live_...\"\n    used_by: [Lookup API, Export API, MCP server]\n    key_prefix: sk_live_\n    obtain: https://app.syftdata.com/dashboard/settings/snippets\n  - type: apiKey\n    in: header\n    name: x-syft-secret-key\n    format: \"x-syft-secret-key: sk_live_...\"\n    used_by: [Lookup API, Export API]\n  - type: apiKey\n    in: body\n    name: secretKey\n    used_by: [Lookup API]\n\
  \  - type: apiKey\n    name: sourceId\n    location: client SDK init / data attribute\n    used_by: [JavaScript tracking SDK]\n    note: Public source identifier used by the browser tracking pixel; not a secret.\n  - type: oauth2\n    name: MCP OAuth (Auth0)\n    issuer: https://syft-studio.us.auth0.com/\n    used_by: [MCP server (Claude, ChatGPT, Claude Code)]\n    scopes_supported: [openid, profile, email, offline_access]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/authentication/syft-data-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Lead Intelligence
- Intent Data
- Website Visitor Identification
- Sales Intelligence
- Go-To-Market
- Analytics
- MCP
---
