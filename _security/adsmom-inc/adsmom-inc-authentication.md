---
api_key_in: []
api_specs:
- filename: adsmom-inc-openapi.json
  format: json
  label: Adsmom REST API
  slug: adsmom-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/openapi/adsmom-inc-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adsmom Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adsmom Inc. secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adsmom Inc.
provider_slug: adsmom-inc
scheme_count: 1
schemes:
- applied_to: '77 of 78 operations declare `security: [{oauth: []}]`. getUsage (GET /api/v1/usage) declares no security in the spec but answers 401 unauthenticated in production — a spec defect, not an open endpoint.'
  bearerFormat: JWT
  name: oauth
  scheme: bearer
  sources:
  - openapi/adsmom-inc-openapi.json
  type: http
slug: adsmom-inc-authentication
source_filename: adsmom-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://app.adsmom.com/.well-known/oauth-authorization-server (RFC 8414, HTTP 200)\n  + https://app.adsmom.com/.well-known/oauth-protected-resource (RFC 9728, HTTP 200)\n  + https://app.adsmom.com/.well-known/oauth-protected-resource/mcp (HTTP 200)\n  + openapi/adsmom-inc-openapi.json securitySchemes\n  + observed 401 challenges on https://api.adsmom.com/api/v1/usage and https://api.adsmom.com/mcp\ndocs: https://adsmom.com/product/api\nsummary:\n  model: oauth2\n  types:\n  - http\n  - oauth2\n  note: >-\n    The OpenAPI declares a single scheme — `oauth`, an HTTP bearer scheme with\n    bearerFormat JWT — and applies it to 77 of 78 operations. The spec understates\n    the real model: the token is issued by a full OAuth 2.0 authorization server\n    at app.adsmom.com that publishes RFC 8414 metadata anonymously. Both the REST\n    API and the MCP server answer unauthenticated requests with an RFC 6750\n    WWW-Authenticate\
  \ challenge carrying `resource_metadata`, so a client can\n    discover the whole auth model from the 401 alone.\n\nschemes:\n- name: oauth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: >-\n    77 of 78 operations declare `security: [{oauth: []}]`. getUsage\n    (GET /api/v1/usage) declares no security in the spec but answers 401\n    unauthenticated in production — a spec defect, not an open endpoint.\n  sources:\n  - openapi/adsmom-inc-openapi.json\n\nauthorization_server:\n  issuer: https://app.adsmom.com\n  authorization_endpoint: https://app.adsmom.com/oauth/authorize\n  token_endpoint: https://app.adsmom.com/oauth/token\n  registration_endpoint: https://app.adsmom.com/oauth/register\n  jwks_uri: https://app.adsmom.com/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n\
  \  - none\n  - client_secret_post\n  scopes_supported:\n  - mcp:invoke\n  - api:read\n  - api:write\n  - billing:read\n  authorization_response_iss_parameter_supported: true\n  dynamic_client_registration: true\n  file: well-known/adsmom-inc-oauth-authorization-server.json\n\nprotected_resources:\n- resource: https://app.adsmom.com\n  authorization_servers:\n  - https://app.adsmom.com\n  scopes_supported:\n  - mcp:invoke\n  file: well-known/adsmom-inc-oauth-protected-resource.json\n- resource: https://app.adsmom.com/mcp\n  authorization_servers:\n  - https://app.adsmom.com/mcp\n  scopes_supported:\n  - mcp:invoke\n  file: well-known/adsmom-inc-mcp-oauth-protected-resource.json\n  note: >-\n    The MCP-scoped protected-resource document names its own `mcp` path as the\n    authorization server; the root document and the WWW-Authenticate challenge\n    both name https://app.adsmom.com. Treat the issuer as https://app.adsmom.com.\n\nchallenges:\n- surface: REST\n  url: https://api.adsmom.com/api/v1/usage\n\
  \  http_status: 401\n  content_type: application/problem+json\n  www_authenticate: Bearer resource_metadata=\"https://app.adsmom.com/.well-known/oauth-protected-resource\"\n- surface: MCP\n  url: https://api.adsmom.com/mcp\n  http_status: 401\n  content_type: application/json\n  www_authenticate: Bearer realm=\"mcp\", resource_metadata=\"https://app.adsmom.com/.well-known/oauth-protected-resource/mcp\"\n\nflows:\n- name: client_credentials\n  use: server-to-server REST access (pipelines, internal tools, scheduled jobs)\n  evidence: >-\n    `client_credentials` is listed in grant_types_supported on the root\n    authorization-server metadata, and the OpenAPI info.description says\n    \"Authenticate with OAuth 2.0 client_credentials\".\n- name: authorization_code\n  use: interactive MCP client connection (Claude, Codex, Cursor, Gemini)\n  pkce: required (S256 is the only code_challenge_method offered)\n  evidence: >-\n    The /mcp-scoped authorization-server metadata offers only authorization_code\n\
  \    + refresh_token with token_endpoint_auth_methods_supported [\"none\"], the\n    public-client shape MCP clients use.\n\ncredentials:\n  provisioning: >-\n    Created by the account holder from the Integrations section of\n    https://app.adsmom.com/. Not self-service outside a paid plan — API and MCP\n    access are included on all paid tiers (see plans/adsmom-inc-plans.yml).\n  rotation: not documented publicly\n  cross_links:\n    scopes: scopes/adsmom-inc-scopes.yml\n    well_known: well-known/adsmom-inc-well-known.yml\n    conventions: conventions/adsmom-inc-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/authentication/adsmom-inc-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Advertising
- Ad Intelligence
- Competitive Intelligence
- Marketing
- Artificial Intelligence
- MCP
- Software-as-a-Service
- OpenAPI
- REST
- Analytics
- Social-Media
- agent-native
---
