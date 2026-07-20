---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Elysium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Elysium Health secures its APIs with openIdConnect, oauth2, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Elysium Health
provider_slug: elysium
scheme_count: 4
schemes:
- authorization_endpoint: https://account.elysiumhealth.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.elysiumhealth.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/26818117694
  jwks_uri: https://account.elysiumhealth.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.elysiumhealth.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/elysium-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://account.elysiumhealth.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- metadata_url: https://www.elysiumhealth.com/.well-known/oauth-authorization-server
  name: OAuth2AuthorizationServerMetadata
  note: Identical payload to the OIDC discovery document.
  rfc: RFC 8414
  sources:
  - well-known/elysium-oauth-authorization-server.json
  type: oauth2
- authorization_endpoint: https://auth.elysiumhealth.com/authorize
  logout_endpoint: https://auth.elysiumhealth.com/v2/logout
  name: Auth0Legacy
  note: An Auth0 tenant (auth.elysiumhealth.com) is still referenced from storefront account links alongside the newer Shopify Customer Accounts flow.
  sources:
  - https://www.elysiumhealth.com/
  type: oauth2
- name: NoAuthStorefrontJSON
  note: /products.json, /products/{handle}.json, /collections/{handle}/products.json and /search?q=&type=product require no authentication (provider-documented read-only browsing).
  sources:
  - https://www.elysiumhealth.com/llms.txt
  type: none
slug: elysium-authentication
source_filename: elysium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.elysiumhealth.com/.well-known/openid-configuration\ndocs: https://www.elysiumhealth.com/llms.txt\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - none\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - jwt-bearer\n  pkce: S256\n  api_key_in: []\n  note: >-\n    Elysium Health publishes no developer API keys. Two authentication surfaces exist: (1) Shopify\n    Customer Account OpenID Connect for shopper identity, and (2) unauthenticated read-only\n    storefront JSON endpoints. The UCP MCP commerce endpoint is unauthenticated at the transport\n    level but requires the calling agent to present a UCP agent profile URI, and requires buyer\n    approval at payment time.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.elysiumhealth.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/26818117694\n  authorization_endpoint:\
  \ https://account.elysiumhealth.com/authentication/oauth/authorize\n  token_endpoint: https://account.elysiumhealth.com/authentication/oauth/token\n  end_session_endpoint: https://account.elysiumhealth.com/authentication/logout\n  jwks_uri: https://account.elysiumhealth.com/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/elysium-openid-configuration.json\n- name: OAuth2AuthorizationServerMetadata\n\
  \  type: oauth2\n  rfc: RFC 8414\n  metadata_url: https://www.elysiumhealth.com/.well-known/oauth-authorization-server\n  note: Identical payload to the OIDC discovery document.\n  sources:\n  - well-known/elysium-oauth-authorization-server.json\n- name: Auth0Legacy\n  type: oauth2\n  authorization_endpoint: https://auth.elysiumhealth.com/authorize\n  logout_endpoint: https://auth.elysiumhealth.com/v2/logout\n  note: >-\n    An Auth0 tenant (auth.elysiumhealth.com) is still referenced from storefront account links\n    alongside the newer Shopify Customer Accounts flow.\n  sources:\n  - https://www.elysiumhealth.com/\n- name: NoAuthStorefrontJSON\n  type: none\n  note: >-\n    /products.json, /products/{handle}.json, /collections/{handle}/products.json and\n    /search?q=&type=product require no authentication (provider-documented read-only browsing).\n  sources:\n  - https://www.elysiumhealth.com/llms.txt\npolicy_urls:\n  op_policy_uri: https://www.shopify.com/legal/privacy\n  op_tos_uri:\
  \ https://www.shopify.com/legal/terms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elysium/refs/heads/main/authentication/elysium-authentication.yml
summary_line: openIdConnect/oauth2/none · 4 schemes
tags:
- Company
- Health
- Longevity
- Supplements
- Consumer Health
- Diagnostics
- Agentic Commerce
- Universal Commerce Protocol
- Shopify
- E-Commerce
- MCP
---
