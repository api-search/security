---
anonymous_access: false
api_key_in: []
api_specs:
- filename: affitor-com-tracking-api-openapi.yml
  format: yaml
  label: Affitor Tracking API
  slug: affitor-com-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affitor-com/openapi/affitor-com-tracking-api-openapi.yml
auth_types: []
description: Authentication methods for Affitor
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Affitor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affitor declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Affitor
provider_slug: affitor-com
scheme_count: 3
schemes:
- evidence: Every server-side call to the tracking API — sales, refunds, and server-mode leads — authenticates with a Bearer token that is unique to your program.
  header: Authorization
  how_to_obtain: A workspace owner opens Program settings → API keys in the Affitor dashboard and selects Generate (or Regenerate); the full key is shown once in that response.
  location: header
  name: Program API key
  type: http-bearer
- evidence: Separately from program keys, Affitor issues agent API keys (prefix agt_ ) to approved tools that read and update programs on a brand's behalf through the /api/agent/v1/... endpoints.
  header: Authorization
  how_to_obtain: Issued by Affitor to approved tools; contact support to obtain.
  location: header
  name: Agent API key
  type: http-bearer
- authorize_url: https://mcp.affitor.com/oauth/authorize
  evidence: Read a brand's program or a partner's data from an AI app – The MCP server, signed in with OAuth as an Affitor user, scope `read`.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Clients register via dynamic client registration at https://mcp.affitor.com/oauth/reg and then perform the authorization code flow with PKCE.
  location: header
  name: MCP server OAuth
  scopes:
  - read
  type: oauth2
slug: affitor-com-authentication
source_filename: affitor-com-authentication.yml
source_heading: Authentication Profile
source_url: https://affitor.com/docs/brand/settings
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://affitor.com/docs/brand/settings\nsources:\n- https://affitor.com/docs/brand/settings\n- https://affitor.com/docs/brand/api-keys\n- https://affitor.com/auth.md\n- https://affitor.com/docs/api-reference/integrations/nextjs-supabase\ndescription: Authentication methods for Affitor\nschemes:\n- type: http-bearer\n  name: Program API key\n  evidence: Every server-side call to the tracking API — sales, refunds, and server-mode leads — authenticates with a Bearer token that is unique\n    to your program.\n  location: header\n  header: Authorization\n  how_to_obtain: A workspace owner opens Program settings → API keys in the Affitor dashboard and selects Generate (or Regenerate); the full key\n    is shown once in that response.\n- type: http-bearer\n  name: Agent API key\n  evidence: Separately from program keys, Affitor issues agent API keys (prefix agt_ ) to approved tools that\
  \ read and update programs on a brand's\n    behalf through the /api/agent/v1/... endpoints.\n  location: header\n  header: Authorization\n  how_to_obtain: Issued by Affitor to approved tools; contact support to obtain.\n- type: oauth2\n  name: MCP server OAuth\n  evidence: Read a brand's program or a partner's data from an AI app – The MCP server, signed in with OAuth as an Affitor user, scope `read`.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.affitor.com/oauth/authorize\n  scopes:\n  - read\n  how_to_obtain: Clients register via dynamic client registration at https://mcp.affitor.com/oauth/reg and then perform the authorization code\n    flow with PKCE.\ndocs: https://affitor.com/docs/brand/settings\n"
source_yaml_url: https://artifacts.apis.io/affitor-com/authentication/affitor-com-authentication.yml
summary_line: 3 schemes
tags:
- Affiliates
- Software-as-a-Service
- Artificial Intelligence
- Marketing
- Affiliate Network
---
