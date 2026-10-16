---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corraldata-openapi-generated.yml
  format: yaml
  label: CorralData API
  slug: corraldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corraldata/refs/heads/main/openapi/_ae-authored/corraldata-openapi-generated.yml
auth_types: []
description: CorralData MCP uses OAuth 2.0 Authorization Code flow with PKCE.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Corraldata Authentication
name_suffix: Authentication
oauth_flows: []
overview: CorralData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CorralData
provider_slug: corraldata
scheme_count: 1
schemes:
- evidence: The CorralData MCP Server uses OAuth 2.0 for authentication.
  flows:
  - authorization_code
  how_to_obtain: Client ID is the public OAuth client ID corral-mcp-client; there is no client secret. The client is a public OAuth client protected by PKCE.
  name: CorralData MCP
  type: oauth2
slug: corraldata-authentication
source_filename: corraldata-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.corraldata.com/kb/mcp/authentication
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.corraldata.com/kb/mcp/authentication\nsources:\n- https://docs.corraldata.com/kb/mcp/authentication\n- https://corraldata.com/guided-onboarding/\n- https://docs.corraldata.com/kb/getting-started/how-corraldata-works\n- https://docs.corraldata.com/kb/getting-started/quickstart\ndescription: CorralData MCP uses OAuth 2.0 Authorization Code flow with PKCE.\nschemes:\n- type: oauth2\n  name: CorralData MCP\n  evidence: The CorralData MCP Server uses OAuth 2.0 for authentication.\n  flows:\n  - authorization_code\n  how_to_obtain: Client ID is the public OAuth client ID corral-mcp-client; there is no client secret. The client is a public OAuth client protected\n    by PKCE.\ndocs: https://docs.corraldata.com/kb/mcp/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corraldata/refs/heads/main/authentication/corraldata-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Analytics
- Healthcare
- AI
- Platform
---
