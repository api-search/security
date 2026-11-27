---
anonymous_access: false
api_key_in: []
api_specs:
- filename: growvib-com-agent-payments-api-openapi.yml
  format: yaml
  label: GrowVib Agent payments API
  slug: growvib-com-agent-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growvib-com/openapi/growvib-com-agent-payments-api-openapi.yml
- filename: growvib-com-catalog-api-openapi.yml
  format: yaml
  label: GrowVib Catalog API
  slug: growvib-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growvib-com/openapi/growvib-com-catalog-api-openapi.yml
auth_types: []
description: Authentication schemes for GrowVib
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GrowVib Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrowVib declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GrowVib
provider_slug: growvib-com
scheme_count: 1
schemes:
- authorize_url: https://api.growvib.com/oauth/authorize
  evidence: OAuth 2.1 with PKCE (the MCP server) – To quote against a user's balance, place orders paid from their wallet, check order status, or top the wallet up, connect to https://api.growvib.com/mcp on that user's behalf. The flow is standard and fully automatic for a compliant MCP client; the only human step is the user's approval.
  header: Authorization
  how_to_obtain: Register a public client via POST https://api.growvib.com/oauth/register (dynamic client registration, token_endpoint_auth_method = none). Then use the authorization code flow with PKCE (response_type=code, scope=mcp) to obtain an access token.
  location: header
  name: OAuth 2.1 with PKCE (MCP server)
  scopes:
  - mcp
  token_url: https://api.growvib.com/oauth/token
  type: oauth2
slug: growvib-com-authentication
source_filename: growvib-com-authentication.yml
source_heading: Authentication Profile
source_url: https://growvib.com/auth.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://growvib.com/auth.md\nsources:\n- https://growvib.com/auth.md\ndescription: Authentication schemes for GrowVib\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE (MCP server)\n  evidence: OAuth 2.1 with PKCE (the MCP server) – To quote against a user's balance, place orders paid from their wallet, check order status,\n    or top the wallet up, connect to https://api.growvib.com/mcp on that user's behalf. The flow is standard and fully automatic for a compliant\n    MCP client; the only human step is the user's approval.\n  location: header\n  header: Authorization\n  token_url: https://api.growvib.com/oauth/token\n  authorize_url: https://api.growvib.com/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: Register a public client via POST https://api.growvib.com/oauth/register (dynamic client registration, token_endpoint_auth_method\n    = none). Then use the authorization\
  \ code flow with PKCE (response_type=code, scope=mcp) to obtain an access token.\ndocs: https://growvib.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/growvib-com/authentication/growvib-com-authentication.yml
summary_line: 1 scheme
tags:
- SMM
- Social Media
- Marketing
- Automation
- Telegram
---
