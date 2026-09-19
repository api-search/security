---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'Fox Factory Holding publishes no developer API keys and no partner API program. The authentication surface it actually serves belongs to its FOX storefront at ridefox.com: an OpenID Connect / OAuth 2.0 customer-account authorization server (operated by Shopify under the FOX shop id) and a UCP/MCP commerce endpoint that is anonymous for catalog and cart work and escalates to buyer approval plus a payment handler at checkout completion.'
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Fox Factory Holding Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fox Factory Holding declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Fox Factory Holding
provider_slug: fox-factory-holding
scheme_count: 4
schemes:
- applies_to: https://ridefox.com/api/ucp/mcp
  description: tools/list and read-only catalog tools answered HTTP 200 with no credential on 2026-09-14. There is no API key, no registration and no developer account.
  evidence:
    method: POST
    status: 200
    url: https://ridefox.com/api/ucp/mcp
  id: anonymous-mcp
  type: none
- applies_to: https://ridefox.com/api/ucp/mcp
  description: Every tools/call must carry a UCP agent profile URI identifying the calling agent. This is an identity declaration, not a secret. Omitting it returns JSON-RPC error -32001 (data.code invalid_profile_url) with HTTP 422.
  evidence:
    method: POST
    note: probe with empty arguments
    status: 422
    url: https://ridefox.com/api/ucp/mcp
  id: ucp-agent-profile
  location: meta["ucp-agent"].profile (JSON body, per-tool-call)
  required: true
  type: agentProfile
- applies_to: https://ridefox.com
  authorization_endpoint: https://shopify.com/authentication/68121624800/oauth/authorize
  description: Buyer (customer account) identity for ridefox.com. The issuer is a Shopify-hosted authorization server scoped to the FOX shop id 68121624800; the discovery documents are served from Fox Factory's own host. The live storefront login at /customer_authentication/login redirects to this authorize endpoint with scope "openid email customer-account-api".
  end_session_endpoint: https://shopify.com/authentication/68121624800/logout
  evidence:
    status: 200
    url: https://ridefox.com/.well-known/openid-configuration
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/68121624800
  jwks_uri: https://shopify.com/authentication/68121624800/.well-known/jwks.json
  openIdConnectUrl: https://ridefox.com/.well-known/openid-configuration
  pkce:
  - S256
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/68121624800/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to: https://ridefox.com
  authorization_servers:
  - https://shopify.com/authentication/68121624800
  bearer_methods_supported:
  - header
  description: RFC 9728 protected-resource metadata declaring ridefox.com as the resource and the Shopify authorization server.
  evidence:
    status: 200
    url: https://ridefox.com/.well-known/oauth-protected-resource
  id: oauth-protected-resource
  resource: https://ridefox.com
  type: oauth2
slug: fox-factory-holding-authentication
source_filename: fox-factory-holding-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://ridefox.com/.well-known/openid-configuration, https://ridefox.com/.well-known/oauth-authorization-server,\n  https://ridefox.com/.well-known/oauth-protected-resource, and anonymous JSON-RPC probes of\n  https://ridefox.com/api/ucp/mcp (all 2026-09-14)\nprovider: Fox Factory Holding\nproviderId: fox-factory-holding\ndescription: >-\n  Fox Factory Holding publishes no developer API keys and no partner API program. The authentication\n  surface it actually serves belongs to its FOX storefront at ridefox.com: an OpenID Connect /\n  OAuth 2.0 customer-account authorization server (operated by Shopify under the FOX shop id) and a\n  UCP/MCP commerce endpoint that is anonymous for catalog and cart work and escalates to buyer\n  approval plus a payment handler at checkout completion.\nschemes:\n  - id: anonymous-mcp\n    type: none\n    applies_to: https://ridefox.com/api/ucp/mcp\n    description: >-\n      tools/list and\
  \ read-only catalog tools answered HTTP 200 with no credential on 2026-09-14. There\n      is no API key, no registration and no developer account.\n    evidence: {url: 'https://ridefox.com/api/ucp/mcp', method: POST, status: 200}\n  - id: ucp-agent-profile\n    type: agentProfile\n    applies_to: https://ridefox.com/api/ucp/mcp\n    location: 'meta[\"ucp-agent\"].profile (JSON body, per-tool-call)'\n    required: true\n    description: >-\n      Every tools/call must carry a UCP agent profile URI identifying the calling agent. This is an\n      identity declaration, not a secret. Omitting it returns JSON-RPC error -32001\n      (data.code invalid_profile_url) with HTTP 422.\n    evidence: {url: 'https://ridefox.com/api/ucp/mcp', method: POST, status: 422, note: 'probe with empty arguments'}\n  - id: shopify-customer-account-oidc\n    type: openIdConnect\n    applies_to: https://ridefox.com\n    openIdConnectUrl: https://ridefox.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/68121624800\n\
  \    authorization_endpoint: https://shopify.com/authentication/68121624800/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/68121624800/oauth/token\n    jwks_uri: https://shopify.com/authentication/68121624800/.well-known/jwks.json\n    end_session_endpoint: https://shopify.com/authentication/68121624800/logout\n    flows: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    id_token_signing_alg: [RS256]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    description: >-\n      Buyer (customer account) identity for ridefox.com. The issuer is a Shopify-hosted authorization\n      server scoped to the FOX shop id 68121624800; the discovery documents are served from Fox\n      Factory's own host. The live storefront login at /customer_authentication/login redirects to\n      this authorize endpoint\
  \ with scope \"openid email customer-account-api\".\n    evidence: {url: 'https://ridefox.com/.well-known/openid-configuration', status: 200}\n  - id: oauth-protected-resource\n    type: oauth2\n    applies_to: https://ridefox.com\n    description: RFC 9728 protected-resource metadata declaring ridefox.com as the resource and the Shopify authorization server.\n    resource: https://ridefox.com\n    authorization_servers: ['https://shopify.com/authentication/68121624800']\n    bearer_methods_supported: [header]\n    evidence: {url: 'https://ridefox.com/.well-known/oauth-protected-resource', status: 200}\npayment_authentication:\n  note: >-\n    Checkout completion is authenticated by the buyer through a UCP payment handler, not by an API\n    credential. Handlers declared in the merchant profile are Google Pay (com.google.pay), Shopify card\n    (dev.shopify.card) and Shop Pay (dev.shopify.shop_pay). The provider's own /llms.txt states an agent\n    must not complete payment without explicit,\
  \ contemporaneous buyer approval.\n  source: https://ridefox.com/.well-known/ucp\ngaps:\n  - No security.txt on any Fox Factory host.\n  - No developer API keys, no partner API program, no first-party developer portal.\n  - dealer.ridefox.com answers HTTP 401 — a credentialed dealer portal with no public documentation.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-factory-holding/refs/heads/main/authentication/fox-factory-holding-authentication.yml
summary_line: 4 schemes
tags:
- Suspension
- Cycling
- Power-Sports
- Manufacturing
- E-Commerce
- MCP
- Agentic Commerce
---
