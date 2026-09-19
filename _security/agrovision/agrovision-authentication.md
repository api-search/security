---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Agrovision Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agrovision declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agrovision
provider_slug: agrovision
scheme_count: 2
schemes:
- applies_to: https://shop.fruitist.com/api/ucp/mcp
  evidence:
    body: '{"jsonrpc":"2.0","id":1,"method":"tools/list"}'
    fetched: '2026-09-13'
    http_status: 200
    method: POST
  id: anonymous-mcp
  note: No Authorization header, no API key and no OAuth challenge was required for tools/list. Every tool still requires a `meta.ucp-agent.profile` URI in its arguments — an agent identity declaration, not a credential.
  type: none
- applies_to: shopper sign-in at https://shop.fruitist.com/account
  authorization_endpoint: https://shopify.com/authentication/64996540577/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/64996540577/logout
  grant_types: []
  id: shopify-customer-account-oidc
  id_token_signing_alg_values:
  - RS256
  issuer: https://shopify.com/authentication/64996540577
  jwks_uri: https://shopify.com/authentication/64996540577/.well-known/jwks.json
  note: Operated by Shopify on behalf of this store, not by Agrovision. The issuer is a Shopify tenant URL. Recorded because it is the only identity surface reachable on a company host.
  openIdConnectUrl: https://shop.fruitist.com/.well-known/openid-configuration
  response_types:
  - code
  token_endpoint: https://shopify.com/authentication/64996540577/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: agrovision-authentication
source_filename: agrovision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://shop.fruitist.com/.well-known/openid-configuration\naid: agrovision-ucp-commerce\nsummary: >-\n  Agrovision publishes no API keys, no developer credentials and no authentication\n  documentation of its own. Two real authentication facts were observed on its storefront host:\n  the UCP MCP endpoint accepts anonymous tools/list and anonymous catalog/cart calls, and the\n  store exposes Shopify's customer-account OpenID Connect authorization server for shopper\n  identity.\nschemes:\n- id: anonymous-mcp\n  type: none\n  applies_to: https://shop.fruitist.com/api/ucp/mcp\n  evidence:\n    method: POST\n    body: '{\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n    http_status: 200\n    fetched: '2026-09-13'\n  note: >-\n    No Authorization header, no API key and no OAuth challenge was required for tools/list.\n    Every tool still requires a `meta.ucp-agent.profile` URI in its arguments — an agent\n    identity\
  \ declaration, not a credential.\n- id: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://shop.fruitist.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/64996540577\n  authorization_endpoint: https://shopify.com/authentication/64996540577/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/64996540577/oauth/token\n  jwks_uri: https://shopify.com/authentication/64996540577/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/64996540577/logout\n  grant_types: []\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  id_token_signing_alg_values:\n  - RS256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  applies_to: shopper sign-in at https://shop.fruitist.com/account\n  note: >-\n    Operated by Shopify on behalf of this store, not by Agrovision. The issuer is a Shopify\n    tenant URL. Recorded because it is the only identity\
  \ surface reachable on a company host.\nabsent:\n- api_keys: >-\n    No developer API key programme, no key prefix, no key issuance page anywhere on\n    fruitist.com or agrovisioncorp.com.\n- mutual_tls: not offered\n- signed_requests: not documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrovision/refs/heads/main/authentication/agrovision-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Agriculture
- Food and Beverage
- Consumer Packaged Goods
- Agriculture Technology
- E-Commerce
- Retail
- Supply Chain
- Agentic Commerce
- Universal Commerce Protocol
---
