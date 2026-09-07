---
anonymous_access: true
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 3Ntech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: 3N TECH secures its APIs with oauth2, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: 3N TECH
provider_slug: 3ntech
scheme_count: 3
schemes:
- applies_to: https://www.3neyecare.com/api/ucp/mcp
  description: 'MCP initialize and tools/list are served with no credential of any kind. tools/call is not open: it requires meta.ucp-agent.profile to carry a fetchable agent profile URI, and a call without one returns JSON-RPC error -32001 invalid_profile_url over HTTP 422. That is an agent-identity requirement, not a bearer credential.'
  evidence: observed 2026-09-05, tools/list HTTP 200 anonymous
  name: anonymous-mcp
  type: none
- authorization_endpoint: https://account.3neyecare.com/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.3neyecare.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/71773126944
  jwks_uri: https://account.3neyecare.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://www.3neyecare.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/3ntech-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://account.3neyecare.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- metadata: https://www.3neyecare.com/.well-known/oauth-authorization-server
  name: shopify-customer-account-oauth2
  rfc: RFC 8414
  sources:
  - well-known/3ntech-oauth-authorization-server.json
  type: oauth2
slug: 3ntech-authentication
source_filename: 3ntech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://www.3neyecare.com/.well-known/openid-configuration,\n  https://www.3neyecare.com/.well-known/oauth-authorization-server,\n  https://www.3neyecare.com/.well-known/oauth-protected-resource,\n  live probe of https://www.3neyecare.com/api/ucp/mcp\nnote: >-\n  Derived from the OAuth/OIDC discovery documents the storefront actually serves and from\n  observed behaviour of the MCP endpoint. 3N TECH publishes no OpenAPI, so there are no\n  securitySchemes to aggregate; these are Shopify Customer Account identity endpoints\n  running under 3N's own hosts.\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n- name: anonymous-mcp\n  type: none\n  applies_to: https://www.3neyecare.com/api/ucp/mcp\n  description: >-\n    MCP initialize and tools/list are served with no credential of any kind. tools/call\n    is not open: it requires meta.ucp-agent.profile\
  \ to carry a fetchable agent profile\n    URI, and a call without one returns JSON-RPC error -32001 invalid_profile_url over\n    HTTP 422. That is an agent-identity requirement, not a bearer credential.\n  evidence: observed 2026-09-05, tools/list HTTP 200 anonymous\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.3neyecare.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/71773126944\n  authorization_endpoint: https://account.3neyecare.com/authentication/oauth/authorize\n  token_endpoint: https://account.3neyecare.com/authentication/oauth/token\n  jwks_uri: https://account.3neyecare.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.3neyecare.com/authentication/logout\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n\
  \  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/3ntech-openid-configuration.json]\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  metadata: https://www.3neyecare.com/.well-known/oauth-authorization-server\n  rfc: RFC 8414\n  sources: [well-known/3ntech-oauth-authorization-server.json]\nprotected_resources:\n- resource: https://www.3neyecare.com\n  authorization_servers:\n  - https://account.3neyecare.com\n  - https://shopify.com/authentication/71773126944\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\n  source: well-known/3ntech-oauth-protected-resource.json\n- resource: https://account.3neyecare.com\n  rfc: RFC 9728\n  source: well-known/3ntech-account-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3ntech/refs/heads/main/authentication/3ntech-authentication.yml
summary_line: oauth2/openIdConnect/none · 3 schemes
tags:
- Company
- Eye Care
- Medical Devices
- Consumer Health
- Contact Lenses
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Manufacturing
---
