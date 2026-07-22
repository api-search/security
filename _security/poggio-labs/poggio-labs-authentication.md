---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Poggio Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Poggio Labs secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Poggio Labs
provider_slug: poggio-labs
scheme_count: 2
schemes:
- authorization_endpoint: https://poggio.io/app/oauth/authorize
  code_challenge_methods:
  - S256
  description: The v2 API and the MCP server authenticate with OAuth 2.0. Organization is inferred automatically from the access token. Dynamic Client Registration (RFC 7591) is supported for AI desktop clients.
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://securetoken.google.com/poggio-production-experiments
  name: OAuth2
  registration_endpoint: https://api.poggio.io/v2/oauth/register
  response_types:
  - code
  sources:
  - well-known/poggio-labs-oauth-authorization-server.json
  token_endpoint: https://api.poggio.io/v2/oauth/token
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
- description: Authenticated endpoints and the MCP server accept a Bearer access token in the Authorization header; intended for quick prototyping and simple scripts where full OAuth is unnecessary overhead.
  name: BearerToken
  scheme: bearer
  sources:
  - https://poggio.io/docs/mcp
  type: http
slug: poggio-labs-authentication
source_filename: poggio-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://poggio.io/docs/api and https://api.poggio.io/.well-known/oauth-authorization-server\ndocs: https://poggio.io/docs/api/v2/oauth/token\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  dynamic_client_registration: true\n  pkce: [S256]\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The v2 API and the MCP server authenticate with OAuth 2.0. Organization is\n    inferred automatically from the access token. Dynamic Client Registration\n    (RFC 7591) is supported for AI desktop clients.\n  issuer: https://securetoken.google.com/poggio-production-experiments\n  authorization_endpoint: https://poggio.io/app/oauth/authorize\n  token_endpoint: https://api.poggio.io/v2/oauth/token\n  registration_endpoint: https://api.poggio.io/v2/oauth/register\n  grant_types: [authorization_code, client_credentials, refresh_token]\n  response_types:\
  \ [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_post]\n  sources: [well-known/poggio-labs-oauth-authorization-server.json]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Authenticated endpoints and the MCP server accept a Bearer access token in\n    the Authorization header; intended for quick prototyping and simple scripts\n    where full OAuth is unnecessary overhead.\n  sources: [https://poggio.io/docs/mcp]\nenterprise_identity:\n  sso: SAML 2.0    # https://poggio.io/docs/admin/saml\n  provisioning: SCIM 2.0  # https://poggio.io/docs/admin/scim\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poggio-labs/refs/heads/main/authentication/poggio-labs-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Ai
- Revenue Intelligence
- Sales
- Account Intelligence
- CRM
- Salesforce
- MCP
- AI Agents
- Enterprise
---
