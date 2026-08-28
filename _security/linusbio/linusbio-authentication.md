---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Linusbio Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinusBio declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: LinusBio
provider_slug: linusbio
scheme_count: 3
schemes:
- applies_to: https://traced.life/api/ucp/mcp
  description: 'The UCP/MCP endpoint accepts unauthenticated JSON-RPC. Verified 2026-08-25: an anonymous POST of tools/list returned HTTP 200 with 13 tools.'
  evidence:
    http_status: 200
    url: https://traced.life/api/ucp/mcp
  id: none-public-mcp
  type: none
- authorization_endpoint: https://account.traced.life/authentication/oauth/authorize
  bearer_methods_supported:
  - header
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
  description: Shopify Customer Accounts identity provider for the traced.life store. Platform-provided, not LinusBio-authored, but served from a LinusBio-controlled domain.
  end_session_endpoint: https://account.traced.life/authentication/logout
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oauth2
  id_token_signing_alg_values:
  - RS256
  issuer: https://shopify.com/authentication/70566805578
  jwks_uri: https://account.traced.life/authentication/.well-known/jwks.json
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  token_endpoint: https://account.traced.life/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- description: OIDC discovery for the same provider; response_types_supported is ["code"] only.
  id: shopify-customer-accounts-oidc
  openIdConnectUrl: https://traced.life/.well-known/openid-configuration
  type: openIdConnect
slug: linusbio-authentication
source_filename: linusbio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://traced.life/.well-known/oauth-authorization-server,\n  https://traced.life/.well-known/oauth-protected-resource,\n  https://traced.life/api/ucp/mcp (tools/list)\nsummary: >-\n  LinusBio publishes no developer authentication documentation of any kind. The only auth\n  surface reachable is the Shopify Customer Accounts OAuth 2.0 / OIDC provider backing the\n  traced.life storefront, discovered from RFC 8414 and RFC 9728 metadata served on that host.\n  The public UCP/MCP commerce endpoint itself requires NO credentials — tools/list and catalog\n  reads answer anonymously — while the customer-scoped MCP surface sits behind that OAuth\n  provider.\n\nschemes:\n- id: none-public-mcp\n  type: none\n  applies_to: https://traced.life/api/ucp/mcp\n  description: >-\n    The UCP/MCP endpoint accepts unauthenticated JSON-RPC. Verified 2026-08-25: an anonymous\n    POST of tools/list returned HTTP 200 with 13 tools.\n  evidence:\n\
  \    url: https://traced.life/api/ucp/mcp\n    http_status: 200\n\n- id: shopify-customer-accounts-oauth2\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  issuer: https://shopify.com/authentication/70566805578\n  authorization_endpoint: https://account.traced.life/authentication/oauth/authorize\n  token_endpoint: https://account.traced.life/authentication/oauth/token\n  end_session_endpoint: https://account.traced.life/authentication/logout\n  jwks_uri: https://account.traced.life/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  bearer_methods_supported:\n  - header\n  id_token_signing_alg_values:\n  - RS256\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  description: >-\n    Shopify Customer Accounts identity provider\
  \ for the traced.life store. Platform-provided,\n    not LinusBio-authored, but served from a LinusBio-controlled domain.\n\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://traced.life/.well-known/openid-configuration\n  description: OIDC discovery for the same provider; response_types_supported is [\"code\"] only.\n\nnot_found:\n  - LinusBio corporate API key or token documentation (no developer program exists)\n  - Any authentication reference on linusbio.com or clearstrandasd.com\n  - mTLS, HTTP basic, or API-key scheme on any probed host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linusbio/refs/heads/main/authentication/linusbio-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Health
- Diagnostics
- Precision Medicine
- Biotechnology
- Exposomics
- Life Sciences
- Autism
- Commerce
- Agents
---
