---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invokary-com-openapi-generated.yml
  format: yaml
  label: Invokary API
  slug: invokary-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invokary-com/openapi/_ae-authored/invokary-com-openapi-generated.yml
auth_types: []
description: Invokary authentication methods
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Invokary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invokary declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Invokary
provider_slug: invokary-com
scheme_count: 1
schemes:
- authorize_url: https://auth.acme.test/authorize
  evidence: 'the client exchanges the code for a token bound to your MCP server, and from then on it sends `Authorization: Bearer <token>` on every request.'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: User signs in and approves on the authorization server, which then issues a token.
  location: header
  name: Bearer
  scopes:
  - projects:read
  - projects:write
  type: http-bearer
slug: invokary-com-authentication
source_filename: invokary-com-authentication.yml
source_heading: Authentication Profile
source_url: https://invokary.com/guides/mcp-oauth-for-saas-connectors.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://invokary.com/guides/mcp-oauth-for-saas-connectors.md\nsources:\n- https://invokary.com/guides/mcp-oauth-for-saas-connectors.md\n- https://invokary.com/security.md\ndescription: Invokary authentication methods\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'the client exchanges the code for a token bound to your MCP server, and from then on it sends `Authorization: Bearer <token>` on\n    every request.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://auth.acme.test/authorize\n  scopes:\n  - projects:read\n  - projects:write\n  how_to_obtain: User signs in and approves on the authorization server, which then issues a token.\ndocs: https://invokary.com/guides/mcp-oauth-for-saas-connectors.md\n"
source_yaml_url: https://artifacts.apis.io/invokary-com/authentication/invokary-com-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- SaaS Connectors
- MCP
- Plugin Directories
- OAuth
---
