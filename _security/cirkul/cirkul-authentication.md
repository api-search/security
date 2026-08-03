---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
- ucp-agent-profile
description: ''
kind: authentication
layout: security
method: probed
name: Cirkul Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cirkul secures its APIs with none, oauth2, openIdConnect, and ucp-agent-profile across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cirkul
provider_slug: cirkul
scheme_count: 4
schemes:
- applies_to: https://drinkcirkul.com/api/mcp
  description: The storefront MCP server answered tools/list with HTTP 200 and no credential. Read and cart-building tools are anonymous; the buyer-approval requirement, not a token, is what gates payment.
  evidence:
    fetched: '2026-08-02'
    http_status: 200
  name: anonymous-storefront-mcp
  type: none
- applies_to: https://drinkcirkul.com/api/ucp/mcp
  description: The UCP shopping MCP endpoint requires the calling agent to present a resolvable UCP agent profile URI before any method, including tools/list, will run. Passed via MCP transport metadata (_meta.ucp-agent.profile, format uri) — the same field is declared on the storefront search_catalog inputSchema.
  evidence:
    error: -32001 UCP discovery failed / invalid_profile_url
    fetched: '2026-08-02'
    http_status: 422
  name: ucp-agent-profile
  type: ucp-agent-profile
- description: OpenID Connect discovery for the Shopify Customer Account API scoped to Cirkul's shop. Backs the customer login at /account/login and subscription self-service pages.
  issuer: https://shopify.com/authentication/5052170330
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://drinkcirkul.com/.well-known/openid-configuration
  sources:
  - well-known/cirkul-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://shopify.com/authentication/5052170330/oauth/authorize
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
  description: RFC 8414 authorization server metadata, same issuer as the OIDC document.
  endSessionUrl: https://shopify.com/authentication/5052170330/logout
  flows:
  - flow: authorizationCode
    pkce: S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  jwksUri: https://shopify.com/authentication/5052170330/.well-known/jwks.json
  name: shopify-customer-account-oauth2
  scopes: scopes/cirkul-scopes.yml
  sources:
  - well-known/cirkul-oauth-authorization-server.json
  subject_types_supported:
  - public
  tokenUrl: https://shopify.com/authentication/5052170330/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
slug: cirkul-authentication
source_filename: cirkul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://drinkcirkul.com/.well-known/openid-configuration\ndocs: https://drinkcirkul.com/agents.md\nnotes: >-\n  Derived from the OAuth 2.0 / OpenID Connect discovery documents Cirkul serves\n  from its own host, not from an OpenAPI (Cirkul publishes none). Two distinct\n  auth postures coexist: the anonymous storefront MCP server needs no credential\n  at all, while customer-account and UCP-transacting surfaces sit behind Shopify's\n  hosted authorization server for shop 5052170330.\n\nsummary:\n  types: [none, oauth2, openIdConnect, ucp-agent-profile]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  bearer_methods_supported: [header]\n\nschemes:\n- name: anonymous-storefront-mcp\n  type: none\n  applies_to: https://drinkcirkul.com/api/mcp\n  description: The storefront MCP server answered tools/list with HTTP 200 and no\n    credential. Read and cart-building tools are anonymous; the buyer-approval\n\
  \    requirement, not a token, is what gates payment.\n  evidence:\n    fetched: '2026-08-02'\n    http_status: 200\n- name: ucp-agent-profile\n  type: ucp-agent-profile\n  applies_to: https://drinkcirkul.com/api/ucp/mcp\n  description: The UCP shopping MCP endpoint requires the calling agent to present a\n    resolvable UCP agent profile URI before any method, including tools/list, will\n    run. Passed via MCP transport metadata (_meta.ucp-agent.profile, format uri) —\n    the same field is declared on the storefront search_catalog inputSchema.\n  evidence:\n    fetched: '2026-08-02'\n    http_status: 422\n    error: '-32001 UCP discovery failed / invalid_profile_url'\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://drinkcirkul.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/5052170330\n  description: OpenID Connect discovery for the Shopify Customer Account API scoped\n    to Cirkul's shop. Backs the customer\
  \ login at /account/login and subscription\n    self-service pages.\n  sources: [well-known/cirkul-openid-configuration.json]\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  description: RFC 8414 authorization server metadata, same issuer as the OIDC\n    document.\n  authorizationUrl: https://shopify.com/authentication/5052170330/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/5052170330/oauth/token\n  endSessionUrl: https://shopify.com/authentication/5052170330/logout\n  jwksUri: https://shopify.com/authentication/5052170330/.well-known/jwks.json\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes:\
  \ scopes/cirkul-scopes.yml\n  sources: [well-known/cirkul-oauth-authorization-server.json]\n\nprotected_resource:\n  resource: https://drinkcirkul.com\n  authorization_servers: [https://shopify.com/authentication/5052170330]\n  bearer_methods_supported: [header]\n  source: well-known/cirkul-oauth-protected-resource.json\n\npayment_authorization:\n  model: buyer-approval\n  description: Payment is never authorized by a token the agent holds. /agents.md,\n    /llms.txt and /robots.txt all state that checkout, payment and order placement\n    require an explicit, contemporaneous human approval step, and that agents unable\n    to obtain it must route through Shop Pay via the Shop skill.\n  handlers: [com.google.pay, dev.shopify.card, dev.shopify.shop_pay]\n  source: well-known/cirkul-ucp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirkul/refs/heads/main/authentication/cirkul-authentication.yml
summary_line: none/oauth2/openIdConnect/ucp-agent-profile · 4 schemes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- Ecommerce
- Retail
- Subscription Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Hydration
---
