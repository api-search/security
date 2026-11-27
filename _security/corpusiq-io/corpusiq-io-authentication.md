---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corpusiq-io-authentication-api-openapi.yml
  format: yaml
  label: CorpusIQ Authentication API
  slug: corpusiq-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-authentication-api-openapi.yml
- filename: corpusiq-io-discovery-api-openapi.yml
  format: yaml
  label: CorpusIQ Discovery API
  slug: corpusiq-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-discovery-api-openapi.yml
- filename: corpusiq-io-mcp-api-openapi.yml
  format: yaml
  label: CorpusIQ MCP API
  slug: corpusiq-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-mcp-api-openapi.yml
- filename: corpusiq-io-usage-api-openapi.yml
  format: yaml
  label: CorpusIQ Usage API
  slug: corpusiq-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-usage-api-openapi.yml
auth_types:
- http
- oauth2-device-flow
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CorpusIQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: CorpusIQ secures its APIs with http and oauth2-device-flow across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CorpusIQ
provider_slug: corpusiq-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: All CorpusIQ API requests require authentication via a Bearer token in the Authorization header. Tokens are scoped to individual users and inherit the user's connected data sources and permissions.
  expiry_signal: '401 Unauthorized with X-Token-Expired: true'
  header: 'Authorization: Bearer <token>'
  issuance:
  - 'Dashboard: Settings → API → Generate Token (displayed once)'
  - 'ChatGPT app / MCP connector: issued by the integration at first use'
  - OAuth 2.0 Device Authorization Grant (RFC 8628) for AI agents
  - Authorization code flow with PKCE (per OpenAPI scheme description)
  name: bearerAuth
  refresh: The MCP server now mints a 30-day refresh token after a successful device or Google OAuth reconnect. (changelog, August 2026)
  scheme: bearer
  sources:
  - openapi/corpusiq-io-openapi.yml
  - https://www.corpusiq.io/docs/api/authentication
  - https://www.corpusiq.io/docs/changelog
  token_lifetime: Tokens have a 60-minute expiry from the time of issuance.
  type: http
slug: corpusiq-io-authentication
source_filename: corpusiq-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.corpusiq.io/docs/api/authentication\ndocs: https://www.corpusiq.io/docs/api/authentication\nsummary:\n  types:\n  - http\n  - oauth2-device-flow\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer <token>'\n  description: All CorpusIQ API requests require authentication via a Bearer token in the Authorization header.\n    Tokens are scoped to individual users and inherit the user's connected data sources and permissions.\n  token_lifetime: Tokens have a 60-minute expiry from the time of issuance.\n  expiry_signal: '401 Unauthorized with X-Token-Expired: true'\n  issuance:\n  - 'Dashboard: Settings → API → Generate Token (displayed once)'\n  - 'ChatGPT app / MCP connector: issued by the integration at first use'\n  - OAuth 2.0 Device Authorization Grant (RFC 8628) for AI agents\n  - Authorization code flow with PKCE (per OpenAPI scheme description)\n\
  \  refresh: The MCP server now mints a 30-day refresh token after a successful device or Google OAuth reconnect.\n    (changelog, August 2026)\n  sources:\n  - openapi/corpusiq-io-openapi.yml\n  - https://www.corpusiq.io/docs/api/authentication\n  - https://www.corpusiq.io/docs/changelog\ndiscovery:\n- https://mcp2.corpusiq.io/.well-known/oauth-protected-resource\n- https://mcp2.corpusiq.io/.well-known/oauth-authorization-server\nguidance: Tokens must only be used on the server side.\nnote: The authentication page also states \"There is no refresh-token flow; simply re-authenticate\", which conflicts\n  with its FAQ and the August 2026 changelog describing refresh tokens. Recorded both; not probed.\n"
source_yaml_url: https://artifacts.apis.io/corpusiq-io/authentication/corpusiq-io-authentication.yml
summary_line: http/oauth2-device-flow · 1 scheme
tags:
- Company
- Artificial Intelligence
- MCP
- Business Intelligence
- Small Business
- Integration
- ChatGPT
- Analytics
---
