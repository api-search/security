---
api_key_in:
- header
api_specs:
- filename: topograph-openapi-original.json
  format: json
  label: Topograph API
  slug: topograph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-openapi-original.json
- filename: topograph-x402-openapi.json
  format: json
  label: Topograph x402 (agentic commerce)
  slug: topograph-x402-agentic-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-x402-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Topograph Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Topograph secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Topograph
provider_slug: topograph
scheme_count: 2
schemes:
- applies_to: REST API (https://api.topograph.co/v2/*)
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/topograph-openapi-original.json
  type: apiKey
- applies_to: designer / MCP (https://api.topograph.co/designer-mcp)
  authorizationUrl: https://clerk.topograph.co/oauth/authorize
  flows:
  - authorizationCode
  - refreshToken
  issuer: https://clerk.topograph.co
  jwksUri: https://clerk.topograph.co/.well-known/jwks.json
  name: OAuth2.1
  pkce: S256
  registrationUrl: https://clerk.topograph.co/oauth/register
  revocationUrl: https://clerk.topograph.co/oauth/token/revoke
  scopes_ref: scopes/topograph-scopes.yml
  sources:
  - https://api.topograph.co/.well-known/oauth-authorization-server
  tokenUrl: https://clerk.topograph.co/oauth/token
  type: oauth2
slug: topograph-authentication
source_filename: topograph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/topograph-openapi-original.json + https://topograph.co/developers/mcp + https://api.topograph.co/.well-known/oauth-authorization-server\ndocs: https://docs.topograph.co\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  note: >-\n    The REST API authenticates with an x-api-key header (workspace key). The designer / MCP surface\n    authenticates with OAuth 2.1 via Clerk (clerk.topograph.co); production API keys are never used\n    by the MCP client.\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: REST API (https://api.topograph.co/v2/*)\n  sources:\n  - openapi/topograph-openapi-original.json\n- name: OAuth2.1\n  type: oauth2\n  applies_to: designer / MCP (https://api.topograph.co/designer-mcp)\n  issuer: https://clerk.topograph.co\n  authorizationUrl: https://clerk.topograph.co/oauth/authorize\n\
  \  tokenUrl: https://clerk.topograph.co/oauth/token\n  revocationUrl: https://clerk.topograph.co/oauth/token/revoke\n  jwksUri: https://clerk.topograph.co/.well-known/jwks.json\n  registrationUrl: https://clerk.topograph.co/oauth/register\n  pkce: S256\n  flows: [authorizationCode, refreshToken]\n  scopes_ref: scopes/topograph-scopes.yml\n  sources:\n  - https://api.topograph.co/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/authentication/topograph-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- KYB
- Company Data
- Business Registers
- Compliance
- Identity Verification
- Beneficial Ownership
- AML
- Due Diligence
- Fintech
---
