---
anonymous_access: false
api_key_in: []
api_specs:
- filename: catchintent-com-discovery-api-openapi.yml
  format: yaml
  label: CatchIntent Discovery API
  slug: catchintent-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-discovery-api-openapi.yml
- filename: catchintent-com-health-api-openapi.yml
  format: yaml
  label: CatchIntent Health API
  slug: catchintent-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-health-api-openapi.yml
- filename: catchintent-com-mcp-api-openapi.yml
  format: yaml
  label: CatchIntent MCP API
  slug: catchintent-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-mcp-api-openapi.yml
- filename: catchintent-com-oauth-api-openapi.yml
  format: yaml
  label: CatchIntent OAuth API
  slug: catchintent-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-oauth-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CatchIntent Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CatchIntent secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CatchIntent
provider_slug: catchintent-com
scheme_count: 1
schemes:
- description: OAuth 2.1 with PKCE. Discover endpoints from https://engine.catchintent.com/.well-known/oauth-authorization-server. Request only the scopes needed for the MCP tools being called.
  flows:
  - authorizationUrl: https://engine.catchintent.com/mcp/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://engine.catchintent.com/mcp/token
  name: mcpOAuth
  sources:
  - openapi/catchintent-com-openapi.json
  type: oauth2
slug: catchintent-com-authentication
source_filename: catchintent-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/catchintent-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://engine.catchintent.com/mcp/authorize\n    tokenUrl: https://engine.catchintent.com/mcp/token\n    scopes: 9\n  description: OAuth 2.1 with PKCE. Discover endpoints from https://engine.catchintent.com/.well-known/oauth-authorization-server.\n    Request only the scopes needed for the MCP tools being called.\n  sources:\n  - openapi/catchintent-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/catchintent-com/authentication/catchintent-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- B2B
- Sales
- Intent Data
- Artificial Intelligence
- Outbound
---
