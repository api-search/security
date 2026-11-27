---
anonymous_access: false
api_key_in: []
api_specs:
- filename: odooconsole-com-discovery-api-openapi.yml
  format: yaml
  label: OConsole Discovery API
  slug: odooconsole-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-discovery-api-openapi.yml
- filename: odooconsole-com-mcp-api-openapi.yml
  format: yaml
  label: OConsole MCP API
  slug: odooconsole-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-mcp-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: OConsole Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OConsole secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OConsole
provider_slug: odooconsole-com
scheme_count: 1
schemes:
- description: Authorization code with PKCE. Clients register themselves at `https://auth.odooconsole.com/oauth2/register` (RFC 7591) — there is no client id to copy out of a dashboard.
  flows:
  - authorizationUrl: https://auth.odooconsole.com/oauth2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.odooconsole.com/oauth2/token
  name: odooconsole
  sources:
  - openapi/odooconsole-com-openapi.json
  type: oauth2
slug: odooconsole-com-authentication
source_filename: odooconsole-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/odooconsole-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: odooconsole\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.odooconsole.com/oauth2/auth\n    tokenUrl: https://auth.odooconsole.com/oauth2/token\n    scopes: 4\n  description: Authorization code with PKCE. Clients register themselves at `https://auth.odooconsole.com/oauth2/register`\n    (RFC 7591) — there is no client id to copy out of a dashboard.\n  sources:\n  - openapi/odooconsole-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/odooconsole-com/authentication/odooconsole-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- ERP
- Hosting
- Odoo
---
