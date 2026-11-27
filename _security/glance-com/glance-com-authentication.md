---
anonymous_access: false
api_key_in: []
api_specs:
- filename: glance-com-openapi-generated.yml
  format: yaml
  label: Glance API
  slug: glance-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glance-com/openapi/_ae-authored/glance-com-openapi-generated.yml
auth_types: []
description: Authentication methods published for Glance MCP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Glance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glance declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Glance
provider_slug: glance-com
scheme_count: 1
schemes:
- authorize_url: https://ember.ailooks.glance.com/authorize
  evidence: The server implements OAuth 2.0 with PKCE, handled automatically by any compliant MCP agent — no manual token management needed.
  flows:
  - authorization_code
  how_to_obtain: Google SSO or anonymous
  name: OAuth 2.0
  scopes:
  - catalog:read
  - selfie:read
  - selfie:write
  - tryon:invoke
  - link:open
  type: oauth2
slug: glance-com-authentication
source_filename: glance-com-authentication.yml
source_heading: Authentication Profile
source_url: https://glance.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://glance.com/.well-known/oauth-authorization-server\nsources:\n- https://glance.com/.well-known/oauth-authorization-server\n- https://glance.com/.well-known/oauth-protected-resource\n- https://docs.glance.com/mcp/mcp/authentication.html\n- https://glance.com/us/glanceai/help/getting-started\ndescription: Authentication methods published for Glance MCP\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The server implements OAuth 2.0 with PKCE, handled automatically by any compliant MCP agent — no manual token management needed.\n  flows:\n  - authorization_code\n  authorize_url: https://ember.ailooks.glance.com/authorize\n  scopes:\n  - catalog:read\n  - selfie:read\n  - selfie:write\n  - tryon:invoke\n  - link:open\n  how_to_obtain: Google SSO or anonymous\ndocs: https://glance.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/glance-com/authentication/glance-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Shopping
- Personalization
- Commerce
- Fashion
---
