---
api_key_in: []
api_specs:
- filename: characterquilt-branding-api-openapi.yml
  format: yaml
  label: CharacterQuilt Branding API
  slug: characterquilt-branding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/openapi/characterquilt-branding-api-openapi.yml
- filename: characterquilt-discovery-api-openapi.yml
  format: yaml
  label: CharacterQuilt Discovery API
  slug: characterquilt-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/openapi/characterquilt-discovery-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Characterquilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: CharacterQuilt declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CharacterQuilt
provider_slug: characterquilt
scheme_count: 0
schemes: []
slug: characterquilt-authentication
source_filename: characterquilt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  live probes of https://mcp.characterquilt.com/api/mcp (401 + WWW-Authenticate),\n  https://mcp.characterquilt.com/.well-known/oauth-protected-resource (200), and\n  https://www.characterquilt.com/branding/{slug}.json (200, anonymous)\nnote: >-\n  CharacterQuilt runs two surfaces with two completely different authentication\n  postures. The public brand-profiles data surface is unauthenticated and\n  CORS-open. The hosted MCP server is OAuth-protected and returns a spec-correct\n  RFC 9728 challenge. Neither surface has a published authentication guide; every\n  fact below was observed on the wire on 2026-08-13.\nsurfaces:\n- name: Brand Profiles (public data surface)\n  base_url: https://www.characterquilt.com\n  auth: none\n  schemes: []\n  evidence:\n    url: https://www.characterquilt.com/branding/stripe.json\n    http_status: 200\n    note: >-\n      Returned 26 KB of JSON with no credential presented.\n      access-control-allow-origin:\
  \ * — readable from any browser origin.\n      strict-transport-security: max-age=63072000.\n- name: CharacterQuilt MCP Server\n  base_url: https://mcp.characterquilt.com\n  endpoint: https://mcp.characterquilt.com/api/mcp\n  auth: oauth2\n  schemes:\n  - type: oauth2\n    name: mcpOAuth\n    profile: OAuth 2.1 bearer, as required by the MCP authorization spec\n    bearer_methods_supported:\n    - header\n    discovery:\n      protected_resource_metadata: https://mcp.characterquilt.com/.well-known/oauth-protected-resource\n      standard: RFC 9728\n      status: 200\n    challenge: >-\n      WWW-Authenticate: Bearer\n      resource_metadata=\"https://mcp.characterquilt.com/.well-known/oauth-protected-resource\"\n    scopes:\n    - read:design_brain\n    - write:generated_artifacts\n    - publish:public_file\n    - read:agent_work\n    - write:agent_work\n    scopes_artifact: scopes/characterquilt-scopes.yml\n  evidence:\n    url: https://mcp.characterquilt.com/api/mcp\n    http_status:\
  \ 401\n    body: '{\"error\":\"unauthorized\"}'\n    note: >-\n      Anonymous POST of jsonrpc tools/list and initialize both return 401 with the\n      RFC 9728 resource_metadata challenge header. GET returns the same. The server\n      is real and reachable; its tool schemas require an authenticated\n      introspection.\nfindings:\n- id: rfc9728-implemented-correctly\n  good: true\n  detail: >-\n    The 401 carries a WWW-Authenticate: Bearer header with a resource_metadata\n    parameter, and that URL serves valid JSON metadata. This is the correct MCP\n    authorization handshake and most MCP servers in the catalog do not do it.\n- id: authorization-server-metadata-unreachable\n  good: false\n  detail: >-\n    The advertised authorization server is https://characterquilt-review-beta.vercel.app,\n    a Vercel PREVIEW deployment rather than a production identity host, and it does\n    not serve RFC 8414 metadata — /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration\
  \ both return HTTP 200 with the Next.js HTML\n    application shell. A conforming MCP client that follows the discovery chain\n    cannot obtain an authorization or token endpoint, so the documented flow cannot\n    be completed by a third party.\n  evidence:\n  - url: https://characterquilt-review-beta.vercel.app/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: text/html\n  - url: https://characterquilt-review-beta.vercel.app/.well-known/openid-configuration\n    http_status: 200\n    content_type: text/html\n- id: no-published-auth-guide\n  good: false\n  detail: >-\n    CharacterQuilt publishes no developer portal, API reference or authentication\n    page. /developers, /docs, /docs/api and /api-docs all return 404 on\n    www.characterquilt.com. Everything above had to be probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/authentication/characterquilt-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketing
- Artificial Intelligence
- AI Agents
- Marketing Automation
- Campaign Management
- Brand Identity
- Computer Use Agents
- Y Combinator
- Data
- MCP
---
