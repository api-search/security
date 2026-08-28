---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Rhone Apparel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rhone Apparel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Rhone Apparel
provider_slug: rhone-apparel
scheme_count: 2
schemes:
- anonymous_read: true
  description: The UCP/MCP endpoint accepts tools/list anonymously. tools/call requires a resolvable UCP agent profile URI supplied in the request meta block; the server fetches it and rejects the call with JSON-RPC -32001 / data.code invalid_profile_url (HTTP 422) when it is missing, and profile_unreachable when it cannot be fetched. This is agent identity, not a bearer secret - no API key is issued to the caller.
  evidence: probed 2026-08-26 - POST tools/list 200, POST tools/call without profile 422
  id: ucp-mcp-agent-profile
  in: body
  location: params.meta['ucp-agent'].profile
  surface: https://rhone.myshopify.com/api/ucp/mcp
  type: agentProfile
- authorization_endpoint: https://account.rhone.com/authentication/oauth/authorize
  bearer_methods_supported:
  - header
  description: Shopify Customer Accounts OIDC, branded on account.rhone.com. Gates the Customer Account API and the Customer Account MCP API for a signed-in Rhone shopper.
  end_session_endpoint: https://account.rhone.com/authentication/logout
  evidence: probed 2026-08-26 - openid-configuration, oauth-authorization-server and oauth-protected-resource all 200
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/2497784
  jwks_uri: https://account.rhone.com/.well-known/jwks.json
  openIdConnectUrl: https://account.rhone.com/.well-known/openid-configuration
  pkce:
  - S256
  protected_resource: https://account.rhone.com
  response_types:
  - code
  token_endpoint: https://account.rhone.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: rhone-apparel-authentication
source_filename: rhone-apparel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://account.rhone.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Rhone has no first-party developer program. Two authentication models are observable on\n  Rhone-controlled hosts, both provided by the Shopify platform under Rhone's own domains.\nschemes:\n  - id: ucp-mcp-agent-profile\n    type: agentProfile\n    surface: https://rhone.myshopify.com/api/ucp/mcp\n    in: body\n    location: params.meta['ucp-agent'].profile\n    description: >-\n      The UCP/MCP endpoint accepts tools/list anonymously. tools/call requires a resolvable UCP\n      agent profile URI supplied in the request meta block; the server fetches it and rejects the\n      call with JSON-RPC -32001 / data.code invalid_profile_url (HTTP 422) when it is missing, and\n      profile_unreachable when it cannot be fetched. This is agent identity, not a bearer secret -\n      no API key is issued to the caller.\n\
  \    anonymous_read: true\n    evidence: probed 2026-08-26 - POST tools/list 200, POST tools/call without profile 422\n  - id: shopify-customer-account-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://account.rhone.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/2497784\n    authorization_endpoint: https://account.rhone.com/authentication/oauth/authorize\n    token_endpoint: https://account.rhone.com/authentication/oauth/token\n    end_session_endpoint: https://account.rhone.com/authentication/logout\n    jwks_uri: https://account.rhone.com/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types: [code]\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    id_token_signing_alg: [RS256]\n    bearer_methods_supported: [header]\n    protected_resource: https://account.rhone.com\n    description: >-\n      Shopify\
  \ Customer Accounts OIDC, branded on account.rhone.com. Gates the Customer Account API\n      and the Customer Account MCP API for a signed-in Rhone shopper.\n    evidence: probed 2026-08-26 - openid-configuration, oauth-authorization-server and oauth-protected-resource all 200\nx-evidence:\n  fetched: '2026-08-26'\n  probes:\n    - url: https://account.rhone.com/.well-known/openid-configuration\n      status: 200\n    - url: https://account.rhone.com/.well-known/oauth-protected-resource\n      status: 200\n    - url: https://rhone.myshopify.com/api/ucp/mcp\n      status: 422\n      note: tools/call without an agent profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhone-apparel/refs/heads/main/authentication/rhone-apparel-authentication.yml
summary_line: 2 schemes
tags:
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Activewear
- Company
---
