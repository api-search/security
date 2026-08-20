---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Superscale Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Superscale secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Superscale
provider_slug: superscale
scheme_count: 2
schemes:
- applies_to: https://mcp.superscale.ai/mcp
  claims_supported:
  - sub
  - iss
  - aud
  - exp
  - iat
  - email
  - name
  - org_id
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://superscale.ai/__clerk/oauth/authorize
    flow: authorizationCode
    refresh_supported: true
    registrationUrl: https://superscale.ai/__clerk/oauth/register
    revocationUrl: https://superscale.ai/__clerk/oauth/token/revoke
    tokenUrl: https://superscale.ai/__clerk/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://superscale.ai/__clerk
  jwks_uri: https://superscale.ai/__clerk/.well-known/jwks.json
  name: superscale-mcp-oauth2
  provider: Clerk
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - profile
  - email
  - public_metadata
  - private_metadata
  - offline_access
  - user:org:read
  service_documentation: https://clerk.com/docs/oauth/scoped-access
  source: https://mcp.superscale.ai/.well-known/oauth-authorization-server
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - none
  - client_secret_post
  type: oauth2
- authorization_data_locations_supported:
  - header
  - body
  authorization_data_types_supported:
  - oauth_scope
  authorization_servers:
  - https://superscale.ai/__clerk
  key_challenges_supported:
  - challenge_algs:
    - S256
    challenge_type: urn:ietf:params:oauth:pkce:code_challenge
  name: superscale-mcp-protected-resource
  resource: https://mcp.superscale.ai/mcp
  scopes_supported:
  - profile
  - email
  source: https://mcp.superscale.ai/.well-known/oauth-protected-resource/mcp
  spec: RFC 9728
  token_introspection_endpoint: https://superscale.ai/__clerk/oauth/token
  token_types_supported:
  - urn:ietf:params:oauth:token-type:access_token
  type: oauth2-protected-resource
slug: superscale-authentication
source_filename: superscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://mcp.superscale.ai/.well-known/oauth-authorization-server,\n  https://mcp.superscale.ai/.well-known/oauth-protected-resource/mcp,\n  live 401 challenge from https://mcp.superscale.ai/mcp\ndocs: https://docs.superscale.ai/integrations/superscale-for-agents\nnote: >-\n  Derived from live, anonymously-served OAuth discovery metadata rather than\n  from an OpenAPI securitySchemes block — Superscale publishes no OpenAPI. The\n  authenticated surface is the product MCP server; the documentation MCP server\n  is anonymous.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: required\n  pkce_methods: [S256]\n  dynamic_client_registration: true\n  identity_provider: Clerk\n  api_keys: false\n  api_keys_note: >-\n    No API key, bearer-token or basic-auth surface is documented anywhere in the\n    340KB docs corpus — \"api key\" and \"bearer\" return zero matches.\nschemes:\n- name: superscale-mcp-oauth2\n\
  \  type: oauth2\n  applies_to: https://mcp.superscale.ai/mcp\n  source: https://mcp.superscale.ai/.well-known/oauth-authorization-server\n  issuer: https://superscale.ai/__clerk\n  provider: Clerk\n  service_documentation: https://clerk.com/docs/oauth/scoped-access\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://superscale.ai/__clerk/oauth/authorize\n    tokenUrl: https://superscale.ai/__clerk/oauth/token\n    revocationUrl: https://superscale.ai/__clerk/oauth/token/revoke\n    registrationUrl: https://superscale.ai/__clerk/oauth/register\n    refresh_supported: true\n  jwks_uri: https://superscale.ai/__clerk/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [client_secret_basic, none, client_secret_post]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported:\
  \ [sub, iss, aud, exp, iat, email, name, org_id]\n  scopes_supported: [openid, profile, email, public_metadata, private_metadata, offline_access, 'user:org:read']\n- name: superscale-mcp-protected-resource\n  type: oauth2-protected-resource\n  spec: RFC 9728\n  resource: https://mcp.superscale.ai/mcp\n  source: https://mcp.superscale.ai/.well-known/oauth-protected-resource/mcp\n  authorization_servers: [https://superscale.ai/__clerk]\n  token_types_supported: ['urn:ietf:params:oauth:token-type:access_token']\n  token_introspection_endpoint: https://superscale.ai/__clerk/oauth/token\n  authorization_data_types_supported: [oauth_scope]\n  authorization_data_locations_supported: [header, body]\n  key_challenges_supported:\n  - challenge_type: 'urn:ietf:params:oauth:pkce:code_challenge'\n    challenge_algs: [S256]\n  scopes_supported: [profile, email]\nchallenge:\n  observed_on: '2026-08-12'\n  request: POST https://mcp.superscale.ai/mcp {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"\
  }\n  http_status: 401\n  body: '{\"error\":\"Unauthorized\"}'\n  headers:\n    www-authenticate: 'Bearer resource_metadata=https://mcp.superscale.ai/.well-known/oauth-protected-resource/mcp'\n    x-clerk-auth-reason: session-token-and-uat-missing\n    x-clerk-auth-status: signed-out\n  assessment: >-\n    A correct RFC 9728 challenge — the 401 names the protected-resource metadata\n    URL, which resolves anonymously and names the authorization server, which in\n    turn publishes RFC 8414 metadata with a registration endpoint and PKCE S256.\n    An agent can complete discovery and dynamic client registration end to end\n    without any human-readable documentation, which is the point of the pattern.\ndownstream_platform_auth:\n  note: >-\n    Separate from Superscale's own auth: the product connects to Meta Ads,\n    Google Ads, TikTok Ads, Shopify, Google Analytics, Instagram and Slack over\n    each platform's own OAuth. Superscale documents that users authorize from\n    the platform's\
  \ own login, never share a password, and can revoke access from\n    the platform; read and write permissions are requested separately, and\n    spend- or delivery-changing write actions are approval-gated inside\n    Superscale.\n  source: https://docs.superscale.ai/integrations/capabilities\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superscale/refs/heads/main/authentication/superscale-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Marketing
- Advertising
- Generative AI
- Creative
- AdTech
- Software-as-a-Service
- Agents
- MCP
- A2A
- Agent Skills
- Advertising Technology
- Video Generation
- Media Buying
---
