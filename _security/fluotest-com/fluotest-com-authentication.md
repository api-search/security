---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fluotest-com-mcp-api-openapi.yml
  format: yaml
  label: FluoTest MCP API
  slug: fluotest-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-mcp-api-openapi.yml
- filename: fluotest-com-status-api-openapi.yml
  format: yaml
  label: FluoTest Status API
  slug: fluotest-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-status-api-openapi.yml
auth_types: []
description: Authentication schemes for FluoTest MCP endpoint
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FluoTest Authentication
name_suffix: Authentication
oauth_flows: []
overview: FluoTest declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FluoTest
provider_slug: fluotest-com
scheme_count: 2
schemes:
- evidence: OAuth 2.1 (recommended for interactive agents).
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Follow the authorization_code + PKCE flow described in the authorization server metadata; the user approves access on a consent screen.
  location: header
  name: OAuth 2.1
  type: http-bearer
- evidence: 'send it as "Authorization: Bearer fluo_…".'
  header: Authorization
  how_to_obtain: Generate a fluo_… key in Settings → Security → API keys and copy the value.
  location: header
  name: API key
  type: apiKey
slug: fluotest-com-authentication
source_filename: fluotest-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fluotest.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fluotest.com/.well-known/oauth-protected-resource\nsources:\n- https://fluotest.com/.well-known/oauth-protected-resource\n- https://fluotest.com/en/docs/mcp-server\n- https://fluotest.com/en/docs/api-reference\n- https://fluotest.com/auth.md\ndescription: Authentication schemes for FluoTest MCP endpoint\nschemes:\n- type: http-bearer\n  name: OAuth 2.1\n  evidence: OAuth 2.1 (recommended for interactive agents).\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  how_to_obtain: Follow the authorization_code + PKCE flow described in the authorization server metadata; the user approves access on a consent\n    screen.\n- type: apiKey\n  name: API key\n  evidence: 'send it as \"Authorization: Bearer fluo_…\".'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a fluo_… key in Settings → Security → API keys and copy the value.\n\
  docs: https://fluotest.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/fluotest-com/authentication/fluotest-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Quiz
- No-Code
- Education
- Marketing
---
