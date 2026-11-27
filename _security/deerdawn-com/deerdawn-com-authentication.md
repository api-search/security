---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deerdawn-com-auth-api-openapi.yml
  format: yaml
  label: DeerDawn Auth API
  slug: deerdawn-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-auth-api-openapi.yml
- filename: deerdawn-com-keys-api-openapi.yml
  format: yaml
  label: DeerDawn Keys API
  slug: deerdawn-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-keys-api-openapi.yml
- filename: deerdawn-com-session-memory-api-openapi.yml
  format: yaml
  label: DeerDawn Session Memory API
  slug: deerdawn-com-session-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-session-memory-api-openapi.yml
- filename: deerdawn-com-system-api-openapi.yml
  format: yaml
  label: DeerDawn System API
  slug: deerdawn-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-system-api-openapi.yml
auth_types: []
description: Authentication methods published by DeerDawn
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DeerDawn Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeerDawn declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DeerDawn
provider_slug: deerdawn-com
scheme_count: 1
schemes:
- evidence: It uses OAuth 2.1 Authorization Code with PKCE through your browser.
  flows:
  - authorization_code
  how_to_obtain: Browser sign‑in via the URL returned by get_auth_status; the hosted endpoint https://api.deerdawn.com/mcp triggers the OAuth flow.
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - context:read
  - context:write
  type: oauth2
slug: deerdawn-com-authentication
source_filename: deerdawn-com-authentication.yml
source_heading: Authentication Profile
source_url: https://deerdawn.com/blog/mcp-tool-list-token-cost
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://deerdawn.com/blog/mcp-tool-list-token-cost\nsources:\n- https://deerdawn.com/blog/mcp-tool-list-token-cost\n- https://deerdawn.com/docs/quickstart\n- https://deerdawn.com/docs/mcp-server\n- https://deerdawn.com/blog/best-ai-workflow-setup-for-coding\ndescription: Authentication methods published by DeerDawn\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: It uses OAuth 2.1 Authorization Code with PKCE through your browser.\n  flows:\n  - authorization_code\n  scopes:\n  - context:read\n  - context:write\n  how_to_obtain: Browser sign‑in via the URL returned by get_auth_status; the hosted endpoint https://api.deerdawn.com/mcp triggers the OAuth\n    flow.\ndocs: https://deerdawn.com/blog/mcp-tool-list-token-cost\n"
source_yaml_url: https://artifacts.apis.io/deerdawn-com/authentication/deerdawn-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Session Memory
- MCP
- Productivity
- Platform
- Company
---
