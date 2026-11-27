---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for MCPulse as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: MCPulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCPulse declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MCPulse
provider_slug: getmcpulse-com
scheme_count: 3
schemes:
- evidence: 'An ingest key is what the SDK sends:


    Authorization: Bearer mp_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
  header: Authorization
  location: header
  name: Ingest key
  type: http-bearer
- evidence: The browser holds a Supabase-issued access token and sends it as a Bearer token to every non-ingest route.
  header: Authorization
  location: header
  name: Dashboard session
  type: http-bearer
- evidence: The MCP endpoint takes an OAuth 2.1 access token, not an ingest key. Your AI client discovers where to authenticate from the `WWW-Authenticate` header on the first 401, sends you to a consent screen, and receives a scoped token.
  header: Authorization
  location: header
  name: MCP OAuth
  type: oauth2
slug: getmcpulse-com-authentication
source_filename: getmcpulse-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getmcpulse.com/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getmcpulse.com/authentication.md\nsources:\n- https://docs.getmcpulse.com/authentication.md\n- https://docs.getmcpulse.com/api-keys/create.md\n- https://docs.getmcpulse.com/api-keys/list.md\n- https://docs.getmcpulse.com/api-keys/revoke.md\ndescription: Authentication schemes for MCPulse as documented.\nschemes:\n- type: http-bearer\n  name: Ingest key\n  evidence: 'An ingest key is what the SDK sends:\n\n\n    Authorization: Bearer mp_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Dashboard session\n  evidence: The browser holds a Supabase-issued access token and sends it as a Bearer token to every non-ingest route.\n  location: header\n  header: Authorization\n- type: oauth2\n  name: MCP OAuth\n  evidence: The MCP endpoint takes an OAuth 2.1 access token, not an ingest key. Your AI client discovers\
  \ where to authenticate from the `WWW-Authenticate`\n    header on the first 401, sends you to a consent screen, and receives a scoped token.\n  location: header\n  header: Authorization\ndocs: https://docs.getmcpulse.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/getmcpulse-com/authentication/getmcpulse-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Analytics
- Monitoring
- SDK
- MCP
---
