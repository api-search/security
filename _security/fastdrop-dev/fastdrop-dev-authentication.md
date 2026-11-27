---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastdrop-dev-health-api-openapi.yml
  format: yaml
  label: FastDrop Health API
  slug: fastdrop-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-health-api-openapi.yml
- filename: fastdrop-dev-mcp-api-openapi.yml
  format: yaml
  label: FastDrop MCP API
  slug: fastdrop-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-mcp-api-openapi.yml
- filename: fastdrop-dev-subregistry-api-openapi.yml
  format: yaml
  label: FastDrop Subregistry API
  slug: fastdrop-dev-subregistry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-subregistry-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: FastDrop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FastDrop secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FastDrop
provider_slug: fastdrop-dev
scheme_count: 2
schemes:
- bearerFormat: fd_
  description: FastDrop API key (starts with fd_). Create one in the dashboard at /app/developer (Developer tab). Grants read access plus write access to your own submissions, votes, reviews, and comments over /mcp. Revoke any time; no scope narrowing on keys - prefer OAuth when a client only needs MCP access.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/fastdrop-dev-openapi.json
  type: http
- description: OAuth 2 for MCP clients (RFC 8414 metadata at /.well-known/oauth-authorization-server, protected-resource metadata at /.well-known/oauth-protected-resource/mcp). Public clients supported (empty client secret on the token endpoint).
  flows:
  - authorizationUrl: https://fastdrop.dev/api/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://fastdrop.dev/api/auth/oauth2/token
  name: FastDropOAuth
  sources:
  - openapi/fastdrop-dev-openapi.json
  type: oauth2
slug: fastdrop-dev-authentication
source_filename: fastdrop-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fastdrop-dev-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: fd_\n  description: FastDrop API key (starts with fd_). Create one in the dashboard at /app/developer\n    (Developer tab). Grants read access plus write access to your own submissions, votes, reviews,\n    and comments over /mcp. Revoke any time; no scope narrowing on keys - prefer OAuth when\n    a client only needs MCP access.\n  sources:\n  - openapi/fastdrop-dev-openapi.json\n- name: FastDropOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fastdrop.dev/api/auth/oauth2/authorize\n    tokenUrl: https://fastdrop.dev/api/auth/oauth2/token\n    scopes: 2\n  description: OAuth 2 for MCP clients (RFC 8414 metadata at /.well-known/oauth-authorization-server,\n    protected-resource metadata at\
  \ /.well-known/oauth-protected-resource/mcp). Public clients\n    supported (empty client secret on the token endpoint).\n  sources:\n  - openapi/fastdrop-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fastdrop-dev/authentication/fastdrop-dev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Launch board
- MCP
- Artificial Intelligence
- Developer Tools
- Platform
---
