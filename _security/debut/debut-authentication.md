---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Debut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Debut declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Debut
provider_slug: debut
scheme_count: 4
schemes:
- applies_to:
  - tools/list
  - search_catalog
  - lookup_catalog
  - get_product
  - create_cart
  - get_cart
  - update_cart
  - cancel_cart
  - create_checkout
  - get_checkout
  - update_checkout
  - cancel_checkout
  id: anonymous
  note: No credential was presented on the probe. The only required request metadata is meta["ucp-agent"].profile — a URI naming the calling agent's UCP profile, which the server fetches and validates. It is agent identification, not authentication; a malformed or unfetchable profile returns JSON-RPC error -32001 profile_malformed.
  type: none
- format: uri
  id: ucp-agent-profile
  location: request body
  note: Required on every tool call. Server-side fetched and content-type checked; this is the mechanism by which the merchant identifies which agent is transacting.
  parameter: meta.ucp-agent.profile
  required: true
  type: agentIdentity
- applies_to:
  - customer account operations
  - get_order (buyer-scoped order retrieval)
  authorization_endpoint: https://account.deinde.com/authentication/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  end_session_endpoint: https://account.deinde.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/75476861220
  jwks_uri: https://account.deinde.com/authentication/.well-known/jwks.json
  note: Operated by Shopify on Debut's behalf. Subject types are public; the resource server metadata at /.well-known/oauth-protected-resource names https://www.deinde.com as the resource and both https://account.deinde.com and the Shopify issuer as authorization servers, with bearer tokens in the Authorization header.
  openIdConnectUrl: https://www.deinde.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  scopes: scopes/debut-scopes.yml
  token_endpoint: https://account.deinde.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to:
  - complete_checkout
  id: buyer-payment-approval
  note: The store's published agent instructions state that agents must not complete payment without contemporaneous buyer consent, and recommend routing payment through Shop Pay via the cross-store Shop skill when consent cannot be obtained in the moment. This is a policy control on top of the payment handlers declared in /.well-known/ucp (Google Pay among them), not a transport credential.
  type: humanApproval
slug: debut-authentication
source_filename: debut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.deinde.com/.well-known/oauth-authorization-server + live MCP tools/list\n  probe of https://www.deinde.com/api/ucp/mcp\n\napi: DEINDE Commerce (UCP MCP)\ndocs: https://www.deinde.com/llms.txt\n\nsummary: >-\n  The DEINDE UCP MCP endpoint is anonymously reachable for discovery, catalog, cart and\n  checkout construction — an unauthenticated tools/list returned all 13 tools with full\n  schemas. There is no API key, and no developer registration. What is gated is money and\n  customer data: completing a checkout requires a buyer-approved payment instrument\n  supplied through a UCP payment handler, and customer-account operations run through the\n  Shopify-operated OAuth 2.0 / OpenID Connect authorization server the store advertises\n  from its own host.\n\nschemes:\n\n- id: anonymous\n  type: none\n  applies_to:\n  - tools/list\n  - search_catalog\n  - lookup_catalog\n  - get_product\n  - create_cart\n  - get_cart\n\
  \  - update_cart\n  - cancel_cart\n  - create_checkout\n  - get_checkout\n  - update_checkout\n  - cancel_checkout\n  note: >-\n    No credential was presented on the probe. The only required request metadata is\n    meta[\"ucp-agent\"].profile — a URI naming the calling agent's UCP profile, which the\n    server fetches and validates. It is agent identification, not authentication; a\n    malformed or unfetchable profile returns JSON-RPC error -32001 profile_malformed.\n\n- id: ucp-agent-profile\n  type: agentIdentity\n  location: request body\n  parameter: meta.ucp-agent.profile\n  required: true\n  format: uri\n  note: >-\n    Required on every tool call. Server-side fetched and content-type checked; this is\n    the mechanism by which the merchant identifies which agent is transacting.\n\n- id: shopify-customer-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.deinde.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/75476861220\n  authorization_endpoint:\
  \ https://account.deinde.com/authentication/oauth/authorize\n  token_endpoint: https://account.deinde.com/authentication/oauth/token\n  end_session_endpoint: https://account.deinde.com/authentication/logout\n  jwks_uri: https://account.deinde.com/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes: scopes/debut-scopes.yml\n  applies_to:\n  - customer account operations\n  - get_order (buyer-scoped order retrieval)\n  note: >-\n    Operated by Shopify on Debut's behalf. Subject types are public; the resource server\n    metadata at /.well-known/oauth-protected-resource names\n    https://www.deinde.com\
  \ as the resource and both https://account.deinde.com and the\n    Shopify issuer as authorization servers, with bearer tokens in the Authorization\n    header.\n\n- id: buyer-payment-approval\n  type: humanApproval\n  applies_to:\n  - complete_checkout\n  note: >-\n    The store's published agent instructions state that agents must not complete payment\n    without contemporaneous buyer consent, and recommend routing payment through Shop Pay\n    via the cross-store Shop skill when consent cannot be obtained in the moment. This is\n    a policy control on top of the payment handlers declared in /.well-known/ucp\n    (Google Pay among them), not a transport credential.\n\ncorporate_site:\n  host: www.debutbiotech.com\n  authentication: none\n  note: >-\n    debutbiotech.com is a Webflow marketing site with no login, no account system and no\n    API. Nothing to authenticate against.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debut/refs/heads/main/authentication/debut-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Biotechnology
- Beauty
- Cosmetics
- Skincare
- Ingredients
- Synthetic Biology
- Artificial Intelligence
- Manufacturing
- Ecommerce
- Agentic Commerce
---
