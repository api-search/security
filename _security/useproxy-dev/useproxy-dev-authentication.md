---
anonymous_access: false
api_key_in: []
api_specs:
- filename: useproxy-dev-openapi-generated.yml
  format: yaml
  label: Proxy API
  slug: useproxy-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useproxy-dev/openapi/_ae-authored/useproxy-dev-openapi-generated.yml
auth_types: []
description: Proxy uses OAuth 2.0 with PKCE and dynamic client registration per the MCP authorization spec.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Proxy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proxy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Proxy
provider_slug: useproxy-dev
scheme_count: 1
schemes:
- evidence: Proxy uses OAuth 2.0 with PKCE and dynamic client registration per the MCP authorization spec.
  header: Authorization
  how_to_obtain: Dynamic client registration with PKCE flow; personal tokens via CLI installer (prefix proxy_).
  location: header
  name: OAuth 2.0 PKCE
  type: http-bearer
slug: useproxy-dev-authentication
source_filename: useproxy-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://useproxy.dev/docs/authentication
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://useproxy.dev/docs/authentication\nsources:\n- https://useproxy.dev/docs/authentication\n- https://useproxy.dev/auth.md\n- https://useproxy.dev/docs/quickstart\n- https://useproxy.dev/docs/ads-mcp-claude\ndescription: Proxy uses OAuth 2.0 with PKCE and dynamic client registration per the MCP authorization spec.\nschemes:\n- type: http-bearer\n  name: OAuth 2.0 PKCE\n  evidence: Proxy uses OAuth 2.0 with PKCE and dynamic client registration per the MCP authorization spec.\n  location: header\n  header: Authorization\n  how_to_obtain: Dynamic client registration with PKCE flow; personal tokens via CLI installer (prefix proxy_).\ndocs: https://useproxy.dev/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/useproxy-dev/authentication/useproxy-dev-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- AI
- Marketing
- MCP
- Proxy
---
