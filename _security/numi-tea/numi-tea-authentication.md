---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Numi Tea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numi Tea declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Numi Tea
provider_slug: numi-tea
scheme_count: 3
schemes:
- applies_to: Shopify customer accounts on account.numitea.com
  authorization_endpoint: https://account.numitea.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.numitea.com/authentication/logout
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer_account_oauth2
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/82698961207
  jwks_uri: https://account.numitea.com/authentication/.well-known/jwks.json
  pkce: required
  pkce_methods:
  - S256
  subject_types:
  - public
  token_endpoint: https://account.numitea.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- id: openid_connect
  note: Same authorization server as customer_account_oauth2; OIDC discovery is served on both numitea.com and account.numitea.com.
  openid_connect_url: https://numitea.com/.well-known/openid-configuration
  type: openIdConnect
- applies_to: https://numitea.com/api/ucp/mcp
  bearer_format: JWT
  evidence: 'Unauthenticated tools/call returned JSON-RPC -32000 "AuthenticationRequired": "Unauthorized: A valid JWT is required to call <tool>." The RFC 9728 protected resource document at /.well-known/oauth-protected-resource declares bearer_methods_supported ["header"] and lists account.numitea.com plus the Shopify issuer as the authorization servers.'
  id: ucp_mcp_bearer
  scheme: bearer
  type: http
slug: numi-tea-authentication
source_filename: numi-tea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://numitea.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/agents/get-started/authentication\nnote: >-\n  Derived from the OIDC/OAuth discovery documents Numi Tea serves on its own hosts\n  and from the observed JSON-RPC auth challenge on the UCP MCP endpoint. Numi Tea\n  publishes no developer-facing API auth documentation of its own; the normative\n  reference is Shopify's agent authentication guide, which the server itself names\n  in its error payload.\n\nschemes:\n  - id: customer_account_oauth2\n    type: oauth2\n    flow: authorization_code\n    pkce: required\n    pkce_methods: [S256]\n    issuer: https://shopify.com/authentication/82698961207\n    authorization_endpoint: https://account.numitea.com/authentication/oauth/authorize\n    token_endpoint: https://account.numitea.com/authentication/oauth/token\n    end_session_endpoint: https://account.numitea.com/authentication/logout\n    jwks_uri:\
  \ https://account.numitea.com/authentication/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg: RS256\n    subject_types: [public]\n    claims:\n      - iss\n      - sub\n      - aud\n      - exp\n      - iat\n      - nonce\n      - sid\n      - email\n      - email_verified\n    applies_to: Shopify customer accounts on account.numitea.com\n  - id: openid_connect\n    type: openIdConnect\n    openid_connect_url: https://numitea.com/.well-known/openid-configuration\n    note: Same authorization server as customer_account_oauth2; OIDC discovery is served on both numitea.com and account.numitea.com.\n  - id: ucp_mcp_bearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to: https://numitea.com/api/ucp/mcp\n    evidence: >-\n      Unauthenticated tools/call\
  \ returned JSON-RPC -32000 \"AuthenticationRequired\":\n      \"Unauthorized: A valid JWT is required to call <tool>.\" The RFC 9728 protected\n      resource document at /.well-known/oauth-protected-resource declares\n      bearer_methods_supported [\"header\"] and lists account.numitea.com plus the\n      Shopify issuer as the authorization servers.\n\nprotected_resource:\n  resource: https://numitea.com\n  authorization_servers:\n    - https://account.numitea.com\n    - https://shopify.com/authentication/82698961207\n  bearer_methods_supported: [header]\n  spec: RFC 9728\n\nanonymous_surface:\n  - path: /api/ucp/mcp (initialize, tools/list)\n    note: Capability discovery is anonymous; every tools/call requires a JWT.\n  - path: /products.json\n  - path: /collections/{handle}/products.json\n  - path: /.well-known/ucp\n  - path: /llms.txt\n\napi_keys: false\napi_keys_note: >-\n  Numi Tea issues no API keys and operates no developer program. There is no\n  signup, no key-provisioning\
  \ surface and no self-serve credential on any Numi Tea\n  host; agent credentials for the UCP endpoint are obtained through Shopify's agent\n  authentication flow, not from Numi Tea.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numi-tea/refs/heads/main/authentication/numi-tea-authentication.yml
summary_line: 3 schemes
tags:
- Tea
- Beverages
- Consumer Packaged Goods
- Retail
- E-Commerce
- Organic
- Fair Trade
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
