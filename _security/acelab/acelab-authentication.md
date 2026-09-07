---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Acelab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acelab declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Acelab
provider_slug: acelab
scheme_count: 5
schemes:
- applies_to: https://acelab-api-prod-178528813198.us-east4.run.app/api
  evidence:
    fetched: '2026-09-06'
    http_status: 401
    url: https://acelab-api-prod-178528813198.us-east4.run.app/api/notification/channel-auth
    www_authenticate: Bearer
  id: product-api-bearer
  method: probed
  note: 'The production API answers unauthenticated requests with 401 and WWW-Authenticate: Bearer. How a caller obtains that bearer token is not published anywhere public; in the shipped web application it is a session token minted after interactive sign-in.'
  scheme: bearer
  type: http
- applies_to: https://acelab-api-prod-178528813198.us-east4.run.app/swagger/v1/swagger.json
  evidence:
    fetched: '2026-09-06'
    http_status: 401
    url: https://acelab-api-prod-178528813198.us-east4.run.app/swagger/v1/swagger.json
    www_authenticate: Basic
  id: swagger-basic
  method: probed
  note: 'The ASP.NET Swagger surface EXISTS and is protected by HTTP Basic auth. This is the single most important finding in this record: the machine-readable contract is published by the server, and the only thing between the catalog and it is a credential we do not have and will not attempt. Sibling paths that do not exist (/openapi.json, /api-docs, /health) return 404 from the same host, which is what distinguishes "gated" from "absent" here.'
  scheme: basic
  type: http
- applies_to: https://app.acelabusa.com/login
  id: platform-sso
  method: searched
  note: '"Microsoft & Google OAuth" is listed as an included permission feature on every published Acelab pricing tier. This is end-user sign-in to the Material Hub application, not API authorization.'
  providers:
  - Microsoft
  - Google
  type: oauth2
- applies_to: https://app.acelabusa.com/login
  id: enterprise-sso
  method: searched
  note: '"Custom SSO & RBAC" and "Enterprise SSO & RBAC" are listed as Enterprise-tier-only items on https://www.acelabusa.com/pricing/architect-designers. The protocol is not named on the public page.'
  type: saml-or-oidc
- applies_to: https://docs.acelabusa.com/mcp
  authorization_endpoint: https://docs.acelabusa.com/mcp/oauth/authorize
  evidence:
    fetched: '2026-09-06'
    http_status: 200
    url: https://docs.acelabusa.com/.well-known/oauth-authorization-server
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  id: docs-mcp-oauth
  issuer: https://docs.acelabusa.com/mcp/oauth
  method: probed
  note: Optional. The docs MCP server answers initialize and tools/list anonymously; this authorization server exists to unlock authenticated/private documentation content. Provided by the Mintlify docs platform on Acelab's host.
  optional: true
  pkce:
  - S256
  registration_endpoint: https://docs.acelabusa.com/mcp/oauth/register
  scopes:
  - mcp:search
  token_endpoint: https://docs.acelabusa.com/mcp/oauth/token
  type: oauth2
slug: acelab-authentication
source_filename: acelab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  Live HTTP probes of the Acelab production API and docs MCP host, plus the published pricing\n  page (https://www.acelabusa.com/pricing/architect-designers) and the Revit integration help\n  center. No OpenAPI securitySchemes were available to derive from — the spec is auth-gated.\nnote: >-\n  Acelab publishes no authentication documentation for developers. Everything below was\n  established by observing WWW-Authenticate challenges on Acelab's own hosts and by reading the\n  end-user/pricing pages. There is no documented key-issuance flow, no developer console and no\n  token endpoint for the product API.\nschemes:\n- id: product-api-bearer\n  type: http\n  scheme: bearer\n  applies_to: https://acelab-api-prod-178528813198.us-east4.run.app/api\n  method: probed\n  evidence:\n    url: https://acelab-api-prod-178528813198.us-east4.run.app/api/notification/channel-auth\n    http_status: 401\n    www_authenticate: Bearer\n\
  \    fetched: '2026-09-06'\n  note: >-\n    The production API answers unauthenticated requests with 401 and WWW-Authenticate: Bearer.\n    How a caller obtains that bearer token is not published anywhere public; in the shipped web\n    application it is a session token minted after interactive sign-in.\n- id: swagger-basic\n  type: http\n  scheme: basic\n  applies_to: https://acelab-api-prod-178528813198.us-east4.run.app/swagger/v1/swagger.json\n  method: probed\n  evidence:\n    url: https://acelab-api-prod-178528813198.us-east4.run.app/swagger/v1/swagger.json\n    http_status: 401\n    www_authenticate: Basic\n    fetched: '2026-09-06'\n  note: >-\n    The ASP.NET Swagger surface EXISTS and is protected by HTTP Basic auth. This is the single\n    most important finding in this record: the machine-readable contract is published by the\n    server, and the only thing between the catalog and it is a credential we do not have and\n    will not attempt. Sibling paths that do not exist (/openapi.json,\
  \ /api-docs, /health) return\n    404 from the same host, which is what distinguishes \"gated\" from \"absent\" here.\n- id: platform-sso\n  type: oauth2\n  applies_to: https://app.acelabusa.com/login\n  method: searched\n  providers:\n  - Microsoft\n  - Google\n  note: >-\n    \"Microsoft & Google OAuth\" is listed as an included permission feature on every published\n    Acelab pricing tier. This is end-user sign-in to the Material Hub application, not API\n    authorization.\n- id: enterprise-sso\n  type: saml-or-oidc\n  applies_to: https://app.acelabusa.com/login\n  method: searched\n  note: >-\n    \"Custom SSO & RBAC\" and \"Enterprise SSO & RBAC\" are listed as Enterprise-tier-only items on\n    https://www.acelabusa.com/pricing/architect-designers. The protocol is not named on the\n    public page.\n- id: docs-mcp-oauth\n  type: oauth2\n  applies_to: https://docs.acelabusa.com/mcp\n  method: probed\n  optional: true\n  issuer: https://docs.acelabusa.com/mcp/oauth\n  authorization_endpoint:\
  \ https://docs.acelabusa.com/mcp/oauth/authorize\n  token_endpoint: https://docs.acelabusa.com/mcp/oauth/token\n  registration_endpoint: https://docs.acelabusa.com/mcp/oauth/register\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  pkce:\n  - S256\n  scopes:\n  - mcp:search\n  evidence:\n    url: https://docs.acelabusa.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-09-06'\n  note: >-\n    Optional. The docs MCP server answers initialize and tools/list anonymously; this\n    authorization server exists to unlock authenticated/private documentation content. Provided\n    by the Mintlify docs platform on Acelab's host.\ngaps:\n- No published API key or token issuance flow for the product API.\n- No developer portal, API reference or authentication guide on any Acelab property.\n- Custom API integration is sold, not self-served — Enterprise tier, \"Contact sales\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acelab/refs/heads/main/authentication/acelab-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Construction
- Architecture
- Building Materials
- Design
- Sustainability
- Product Data
- AECO
- Revit
- Specification
---
