---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Zbiotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZBiotics declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: ZBiotics
provider_slug: zbiotics
scheme_count: 4
schemes:
- description: No Authorization header is required or accepted for tool discovery. A bare POST returned the full 13-tool manifest with input schemas.
  evidence:
    http_status: 200
    method: POST
    note: tools/list returned 13 tools with no credential supplied.
    url: https://zbiotics.com/api/ucp/mcp
  id: ucp-mcp-discovery-anonymous
  scope: tools/list, initialize
  surface: https://zbiotics.com/api/ucp/mcp
  type: none
  verified: probed
- description: Not a bearer credential and not an API key - a dereferenceable identity. Every tool's inputSchema requires meta["ucp-agent"]["profile"], and the store performs a live outbound GET of that URI on each call. Omitting it returns -32001 invalid_profile_url (HTTP 422); supplying a URI the store cannot fetch returns -32001 profile_unreachable (HTTP 422). An agent must therefore publish a reachable profile document before it can transact.
  evidence:
    http_status: 422
    method: POST
    note: Observed twice - once with meta omitted (invalid_profile_url) and once with a profile URI that does not resolve (profile_unreachable).
    url: https://zbiotics.com/api/ucp/mcp
  id: ucp-agent-profile
  scope: tools/call (all 13 tools)
  surface: https://zbiotics.com/api/ucp/mcp
  type: agent-profile-uri
  verified: probed
- bearer_format: JWT
  description: get_order refused an anonymous call with -32000 AuthenticationRequired, HTTP 403, and a message naming the tool and linking https://shopify.dev/docs/agents/get-started/authentication. The token is a customer-account JWT obtained through the OIDC flow below, scope customer-account-mcp-api:full.
  evidence:
    http_status: 403
    method: POST
    url: https://zbiotics.com/api/ucp/mcp
  id: customer-account-jwt
  scheme: bearer
  scope: get_order (and, by the platform's documentation, other customer-scoped tools)
  surface: https://zbiotics.com/api/ucp/mcp
  type: http
  verified: probed
- authorization_endpoint: https://account.zbiotics.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.zbiotics.com/authentication/logout
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/11751391332
  jwks_uri: https://account.zbiotics.com/authentication/.well-known/jwks.json
  note: This is Shopify's Customer Accounts identity, exposed on the merchant's own hosts. The op_policy_uri and op_tos_uri in the document point at shopify.com legal pages, which is the honest tell that the identity provider is the platform rather than ZBiotics itself; the authorization and token endpoints are nevertheless served on account.zbiotics.com.
  openIdConnectUrl: https://zbiotics.com/.well-known/openid-configuration
  pkce:
    required_methods:
    - S256
  response_types_supported:
  - code
  scopes: scopes/zbiotics-scopes.yml
  subject_types_supported:
  - public
  surface: https://account.zbiotics.com
  token_endpoint: https://account.zbiotics.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
slug: zbiotics-authentication
source_filename: zbiotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://zbiotics.com/.well-known/openid-configuration,\n  https://zbiotics.com/.well-known/oauth-protected-resource,\n  https://zbiotics.com/api/ucp/mcp (tools/list, anonymous)\ndocs: https://zbiotics.com/agents.md\nsummary: >-\n  ZBiotics runs a three-tier posture, established by probing rather than by reading a docs page.\n  DISCOVERY on the UCP MCP endpoint is anonymous - tools/list and initialize answered a POST with\n  no credential. INVOCATION is not: tools/call requires meta[\"ucp-agent\"][\"profile\"] to be a URI\n  the store can actually fetch, and it performs a live outbound GET of that document on every\n  call. ORDER-SCOPED tools require a customer-account JWT on top of that. The customer account\n  surface is OpenID Connect: zbiotics.com and account.zbiotics.com both serve an OIDC discovery\n  document with authorization_code + PKCE S256 and a jwks_uri. There is no API-key programme, no\n  developer registration,\
  \ and no published client-credentials flow.\nderived_from: probed discovery documents; the provider publishes no OpenAPI securitySchemes.\nschemes:\n- id: ucp-mcp-discovery-anonymous\n  type: none\n  surface: https://zbiotics.com/api/ucp/mcp\n  scope: tools/list, initialize\n  description: >-\n    No Authorization header is required or accepted for tool discovery. A bare POST returned the\n    full 13-tool manifest with input schemas.\n  verified: probed\n  evidence:\n    url: https://zbiotics.com/api/ucp/mcp\n    method: POST\n    http_status: 200\n    note: tools/list returned 13 tools with no credential supplied.\n- id: ucp-agent-profile\n  type: agent-profile-uri\n  surface: https://zbiotics.com/api/ucp/mcp\n  scope: tools/call (all 13 tools)\n  description: >-\n    Not a bearer credential and not an API key - a dereferenceable identity. Every tool's\n    inputSchema requires meta[\"ucp-agent\"][\"profile\"], and the store performs a live outbound GET\n    of that URI on each call.\
  \ Omitting it returns -32001 invalid_profile_url (HTTP 422); supplying\n    a URI the store cannot fetch returns -32001 profile_unreachable (HTTP 422). An agent must\n    therefore publish a reachable profile document before it can transact.\n  verified: probed\n  evidence:\n    url: https://zbiotics.com/api/ucp/mcp\n    method: POST\n    http_status: 422\n    note: >-\n      Observed twice - once with meta omitted (invalid_profile_url) and once with a profile URI\n      that does not resolve (profile_unreachable).\n- id: customer-account-jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  surface: https://zbiotics.com/api/ucp/mcp\n  scope: get_order (and, by the platform's documentation, other customer-scoped tools)\n  description: >-\n    get_order refused an anonymous call with -32000 AuthenticationRequired, HTTP 403, and a\n    message naming the tool and linking\n    https://shopify.dev/docs/agents/get-started/authentication. The token is a customer-account\n    JWT obtained\
  \ through the OIDC flow below, scope customer-account-mcp-api:full.\n  verified: probed\n  evidence:\n    url: https://zbiotics.com/api/ucp/mcp\n    method: POST\n    http_status: 403\n- id: shopify-customer-account-oidc\n  type: openIdConnect\n  surface: https://account.zbiotics.com\n  openIdConnectUrl: https://zbiotics.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/11751391332\n  authorization_endpoint: https://account.zbiotics.com/authentication/oauth/authorize\n  token_endpoint: https://account.zbiotics.com/authentication/oauth/token\n  end_session_endpoint: https://account.zbiotics.com/authentication/logout\n  jwks_uri: https://account.zbiotics.com/authentication/.well-known/jwks.json\n  flows: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types_supported: [code]\n  pkce:\n    required_methods: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported:\
  \ [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: scopes/zbiotics-scopes.yml\n  verified: probed\n  note: >-\n    This is Shopify's Customer Accounts identity, exposed on the merchant's own hosts. The\n    op_policy_uri and op_tos_uri in the document point at shopify.com legal pages, which is the\n    honest tell that the identity provider is the platform rather than ZBiotics itself; the\n    authorization and token endpoints are nevertheless served on account.zbiotics.com.\nprotected_resources:\n- resource: https://zbiotics.com\n  authorization_servers:\n  - https://account.zbiotics.com\n  - https://shopify.com/authentication/11751391332\n  bearer_methods_supported: [header]\n  spec: RFC 9728\n  file: well-known/zbiotics-oauth-protected-resource.json\n- resource: https://account.zbiotics.com\n  spec: RFC 9728\n  file: well-known/zbiotics-account-oauth-protected-resource.json\ngaps:\n- No security.txt\
  \ on any host (404 on zbiotics.com, account.zbiotics.com, zbiotics.myshopify.com, privacy.zbiotics.com).\n- No published developer credential lifecycle - no key issuance, rotation, or revocation documentation.\n- >-\n  Outside of the order tools there is no per-agent credential, so for catalog, cart and checkout\n  the only identity signal available to the store is the ucp-agent profile URI it dereferences -\n  strong enough to require an agent to be publicly identifiable, but not a secret and not revocable\n  per key.\n- >-\n  Nothing on a ZBiotics-controlled page documents any of this. The authentication path is stated\n  only inside a live error message, which links the platform vendor's docs rather than the\n  provider's own.\nx-evidence:\n  fetched: '2026-09-05'\n  probes:\n  - url: https://zbiotics.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://account.zbiotics.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://zbiotics.com/.well-known/oauth-protected-resource\n\
  \    http_status: 200\n  - url: https://zbiotics.com/api/ucp/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zbiotics/refs/heads/main/authentication/zbiotics-authentication.yml
summary_line: 4 schemes
tags:
- Biotechnology
- Probiotics
- Consumer Health
- Direct to Consumer
- E-Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Company
---
