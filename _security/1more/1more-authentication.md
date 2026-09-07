---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 1More Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 1MORE secures its APIs with none, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 1MORE
provider_slug: 1more
scheme_count: 3
schemes:
- applies_to:
  - https://usa.1more.com/api/ucp/mcp
  - https://usa.1more.com/products.json
  - https://usa.1more.com/collections/{handle}/products.json
  - https://usa.1more.com/products/{handle}.json
  evidence: probed 2026-09-05, HTTP 200 with no Authorization header
  name: anonymous-agent-commerce
  sources:
  - mcp/1more-ucp-tools-list.json
  type: none
- bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://shopify.com/authentication/11404626/oauth/authorize
    code_challenge_methods_supported:
    - S256
    endSessionEndpoint: https://shopify.com/authentication/11404626/logout
    flow: authorizationCode
    issuer: https://shopify.com/authentication/11404626
    jwksUri: https://shopify.com/authentication/11404626/.well-known/jwks.json
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://shopify.com/authentication/11404626/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
  name: shopify-customer-account-oauth2
  protected_resource: https://usa.1more.com
  scheme: bearer
  sources:
  - well-known/1more-openid-configuration.json
  - well-known/1more-oauth-authorization-server.json
  - well-known/1more-oauth-protected-resource.json
  type: oauth2
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  id_token_signing_alg_values_supported:
  - RS256
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://usa.1more.com/.well-known/openid-configuration
  sources:
  - well-known/1more-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: 1more-authentication
source_filename: 1more-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://usa.1more.com/.well-known/openid-configuration,\n  https://usa.1more.com/.well-known/oauth-authorization-server,\n  https://usa.1more.com/.well-known/oauth-protected-resource,\n  https://usa.1more.com/api/ucp/mcp (anonymous tools/list, HTTP 200)\nnote: >-\n  1MORE publishes no developer API and therefore no API-key programme. Two distinct\n  auth postures exist on its storefront host and they should not be conflated. (1) The\n  agent commerce surface - the MCP endpoint at /api/ucp/mcp and the read-only product\n  JSON endpoints - is ANONYMOUS: tools/list, initialize, /products.json and\n  /collections/{handle}/products.json all answered HTTP 200 with no credentials on\n  2026-09-05. Authorization for a purchase is not a token; it is a contemporaneous\n  human buyer approval at the payment step, stated in the store's own agents.md.\n  (2) Shopper accounts use OAuth 2.0 authorization-code + PKCE against Shopify's\n\
  \  customer-account authorization server, discovered from RFC 8414 / OIDC metadata\n  served on 1MORE's own host but issued by shopify.com on 1MORE's behalf.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  agent_surface_auth: none\n  human_approval_required_for: [complete_checkout]\nschemes:\n- name: anonymous-agent-commerce\n  type: none\n  applies_to:\n  - https://usa.1more.com/api/ucp/mcp\n  - https://usa.1more.com/products.json\n  - https://usa.1more.com/collections/{handle}/products.json\n  - https://usa.1more.com/products/{handle}.json\n  evidence: probed 2026-09-05, HTTP 200 with no Authorization header\n  sources:\n  - mcp/1more-ucp-tools-list.json\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  scheme: bearer\n  bearer_methods_supported:\n  - header\n  flows:\n  - flow: authorizationCode\n    issuer: https://shopify.com/authentication/11404626\n    authorizationUrl: https://shopify.com/authentication/11404626/oauth/authorize\n\
  \    tokenUrl: https://shopify.com/authentication/11404626/oauth/token\n    jwksUri: https://shopify.com/authentication/11404626/.well-known/jwks.json\n    endSessionEndpoint: https://shopify.com/authentication/11404626/logout\n    code_challenge_methods_supported:\n    - S256\n    token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    scopes:\n    - openid\n    - email\n    - customer-account-api:full\n    - customer-account-mcp-api:full\n  protected_resource: https://usa.1more.com\n  sources:\n  - well-known/1more-openid-configuration.json\n  - well-known/1more-oauth-authorization-server.json\n  - well-known/1more-oauth-protected-resource.json\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://usa.1more.com/.well-known/openid-configuration\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n\
  \  sources:\n  - well-known/1more-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1more/refs/heads/main/authentication/1more-authentication.yml
summary_line: none/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
