---
api_key_in: []
api_specs:
- filename: precog-public-http-api-openapi.yaml
  format: yaml
  label: Precog Public HTTP API
  slug: precog-public-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-public-http-api-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Precog Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Precog secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Precog
provider_slug: precog
scheme_count: 2
schemes:
- description: All Precog public/admin/metadata HTTP API operations require an HTTP Bearer token (opaque access token). Applied globally in every spec.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/precog-public-http-api-openapi.yaml
  - openapi/precog-admin-http-api-openapi.yaml
  - openapi/precog-metadata-http-api-openapi.yaml
  surface: Public HTTP REST API
  type: http
- authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize
  description: 'The MCP server at studio.precog.cloud is secured with OAuth 2.0 (PKCE S256), supporting authorization_code, client_credentials and refresh_token grants, dynamic client registration (RFC 7591), and RFC 8414 / RFC 9728 discovery metadata. Scopes: synesis:mcp, admin:read, admin:write.'
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  name: PrecogMcpOAuth
  registrationUrl: https://studio.precog.cloud/api/mcp/oauth/register
  sources:
  - https://studio.precog.cloud/.well-known/oauth-authorization-server
  surface: Model Context Protocol server
  tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token
  type: oauth2
slug: precog-authentication
source_filename: precog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  openapi/precog-public-http-api-openapi.yaml,\n  openapi/precog-admin-http-api-openapi.yaml,\n  openapi/precog-metadata-http-api-openapi.yaml,\n  https://studio.precog.cloud/.well-known/oauth-authorization-server\ndocs: https://studio.precog.cloud/docs/\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  human_login:\n  - Google\n  - Microsoft\n  - Email\n  - Magic Link\n  - Enterprise SSO\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  surface: Public HTTP REST API\n  description: >-\n    All Precog public/admin/metadata HTTP API operations require an HTTP Bearer\n    token (opaque access token). Applied globally in every spec.\n  sources:\n  - openapi/precog-public-http-api-openapi.yaml\n  - openapi/precog-admin-http-api-openapi.yaml\n  - openapi/precog-metadata-http-api-openapi.yaml\n- name: PrecogMcpOAuth\n\
  \  type: oauth2\n  surface: Model Context Protocol server\n  description: >-\n    The MCP server at studio.precog.cloud is secured with OAuth 2.0 (PKCE S256),\n    supporting authorization_code, client_credentials and refresh_token grants,\n    dynamic client registration (RFC 7591), and RFC 8414 / RFC 9728 discovery\n    metadata. Scopes: synesis:mcp, admin:read, admin:write.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize\n  tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token\n  registrationUrl: https://studio.precog.cloud/api/mcp/oauth/register\n  sources:\n  - https://studio.precog.cloud/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/authentication/precog-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Data Integration
- ETL
- Artificial Intelligence
- Semantic Layer
- Model Context Protocol
- Data Pipelines
- Analytics
- Enterprise
---
