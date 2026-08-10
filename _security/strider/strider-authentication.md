---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Strider Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Strider secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Strider
provider_slug: strider
scheme_count: 2
schemes:
- applies_to: https://app.striderintel.com/app-api/mcp
  bearer_challenge: 'WWW-Authenticate: Bearer resource_metadata="https://app.striderintel.com/.well-known/oauth-protected-resource/app-api/mcp"'
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://app.striderintel.com/app-api/mcp/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.striderintel.com/app-api/mcp/oauth/token
    scopes: {}
    tokenUrl: https://app.striderintel.com/app-api/mcp/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://app.striderintel.com
  name: StriderMcpOAuth
  registration_endpoint: https://app.striderintel.com/app-api/mcp/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://app.striderintel.com/app-api/mcp/oauth/revoke
  revocation_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  sources:
  - well-known/strider-oauth-authorization-server.json
  - well-known/strider-oauth-protected-resource-mcp.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  type: oauth2
- applies_to: https://api.striderintel.com/
  name: StriderShieldApi
  note: The Shield API host answers HTTP 403 for every path including a random control path. No authentication scheme, key-issuance flow or reference is published anonymously, so none is asserted here. Strider markets Shield as "delivered via API" for SIEM/DLP integration; obtaining the contract requires a customer agreement.
  status: gated
  type: unknown
slug: strider-authentication
source_filename: strider-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://app.striderintel.com/.well-known/oauth-authorization-server\nnote: >-\n  Strider publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  built entirely from the provider's own RFC 8414 and RFC 9728 discovery documents plus the\n  observed WWW-Authenticate challenge — machine-readable auth metadata Strider serves itself.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  scopes_published: false\nschemes:\n- name: StriderMcpOAuth\n  type: oauth2\n  issuer: https://app.striderintel.com\n  applies_to: https://app.striderintel.com/app-api/mcp\n  sources:\n  - well-known/strider-oauth-authorization-server.json\n  - well-known/strider-oauth-protected-resource-mcp.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.striderintel.com/app-api/mcp/oauth/authorize\n    tokenUrl: https://app.striderintel.com/app-api/mcp/oauth/token\n  \
  \  refreshUrl: https://app.striderintel.com/app-api/mcp/oauth/token\n    scopes: {}\n  registration_endpoint: https://app.striderintel.com/app-api/mcp/oauth/register\n  revocation_endpoint: https://app.striderintel.com/app-api/mcp/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  revocation_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  dynamic_client_registration: true\n  bearer_challenge: >-\n    WWW-Authenticate: Bearer\n    resource_metadata=\"https://app.striderintel.com/.well-known/oauth-protected-resource/app-api/mcp\"\n- name: StriderShieldApi\n  type: unknown\n  applies_to: https://api.striderintel.com/\n  status: gated\n  note: >-\n    The Shield API host answers HTTP 403 for every path including a random control path.\n    No authentication scheme, key-issuance\
  \ flow or reference is published anonymously, so\n    none is asserted here. Strider markets Shield as \"delivered via API\" for SIEM/DLP\n    integration; obtaining the contract requires a customer agreement.\ngaps:\n- No scopes_supported in the authorization server metadata — no published scope vocabulary.\n- No /.well-known/openid-configuration; the server is OAuth 2.1, not OIDC.\n- No public authentication documentation page for either the MCP server or the Shield API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strider/refs/heads/main/authentication/strider-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Strategic Intelligence
- Threat Intelligence
- Risk Management
- Security
- Supply Chain
- Due Diligence
- Open Source Intelligence
- Artificial Intelligence
- Geopolitical Risk
---
