---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oranoai-com-openapi-generated.yml
  format: yaml
  label: ORANO API
  slug: oranoai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oranoai-com/openapi/_ae-authored/oranoai-com-openapi-generated.yml
auth_types: []
description: Authentication for ORANO MCP uses a personal key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ORANO Authentication
name_suffix: Authentication
oauth_flows: []
overview: ORANO declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ORANO
provider_slug: oranoai-com
scheme_count: 1
schemes:
- evidence: Add it with claude mcp add --transport http and pass your key in an Authorization header.
  header: Authorization
  how_to_obtain: Subscribe to the $5/month web plan and copy the personal ORANO MCP key from the access page (shown once).
  location: header
  name: Authorization
  type: http-bearer
slug: oranoai-com-authentication
source_filename: oranoai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://oranoai.com/blog/connect-orano-claude-code-mcp.html
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://oranoai.com/blog/connect-orano-claude-code-mcp.html\nsources:\n- https://oranoai.com/blog/connect-orano-claude-code-mcp.html\n- https://oranoai.com/blog/connect-orano-cursor-mcp.html\ndescription: Authentication for ORANO MCP uses a personal key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Add it with claude mcp add --transport http and pass your key in an Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Subscribe to the $5/month web plan and copy the personal ORANO MCP key from the access page (shown once).\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://oranoai.com/blog/connect-orano-claude-code-mcp.html\n"
source_yaml_url: https://artifacts.apis.io/oranoai-com/authentication/oranoai-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Video
- Content
- Platform
- Company
---
