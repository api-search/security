---
anonymous_access: false
api_key_in: []
api_specs:
- filename: liftmcp-com-openapi-generated.yml
  format: yaml
  label: LiftMCP API
  slug: liftmcp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liftmcp-com/openapi/_ae-authored/liftmcp-com-openapi-generated.yml
auth_types: []
description: LiftMCP uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LiftMCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiftMCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LiftMCP
provider_slug: liftmcp-com
scheme_count: 1
schemes:
- evidence: 'When configuring an AI client, the key is used as a Bearer token in the Authorization header: Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: It is generated once when you verify your domain and shown once — LiftMCP does not display the full key again after that.
  location: header
  name: Bearer
  type: http-bearer
slug: liftmcp-com-authentication
source_filename: liftmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.liftmcp.com/mcp-servers/setup-and-configuration/16-managing-api-key
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.liftmcp.com/mcp-servers/setup-and-configuration/16-managing-api-key\nsources:\n- https://help.liftmcp.com/mcp-servers/setup-and-configuration/16-managing-api-key\n- https://help.liftmcp.com/account-and-team/25-enabling-mfa\n- https://help.liftmcp.com/getting-started/01-what-is-liftmcp\n- https://help.liftmcp.com/getting-started/02-what-is-mcp\ndescription: LiftMCP uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'When configuring an AI client, the key is used as a Bearer token in the Authorization header: Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: It is generated once when you verify your domain and shown once — LiftMCP does not display the full key again after that.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other\
  \ authentication schemes are documented on the provided pages.\ndocs: https://help.liftmcp.com/mcp-servers/setup-and-configuration/16-managing-api-key\n"
source_yaml_url: https://artifacts.apis.io/liftmcp-com/authentication/liftmcp-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- MCP
- Web
- Integration
---
