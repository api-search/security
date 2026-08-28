---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Rad Power Bikes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rad Power Bikes declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Rad Power Bikes
provider_slug: rad-power-bikes
scheme_count: 2
schemes:
- applies_to: https://www.radpowerbikes.com/api/ucp/mcp
  description: The UCP shopping MCP endpoint accepts unauthenticated JSON-RPC. Requests carry a meta.ucp-agent.profile URI identifying the calling agent rather than a bearer token. Payment credentials are supplied per-checkout as payment instruments issued by a payment handler (Shop Pay, Shopify card, Google Pay), not as an account credential.
  evidence:
    http_status: 200
    probed: '2026-08-26'
  id: anonymous-mcp
  type: none
- authorization_endpoint: https://account.radpowerbikes.com/authentication/oauth/authorize
  description: Shopify Customer Accounts OIDC, provisioned for shop 7999645 and served from the merchant's own account.radpowerbikes.com host. Client registration is not open to the public; these are the credentials a storefront/app uses on the buyer's behalf.
  end_session_endpoint: https://account.radpowerbikes.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/7999645
  jwks_uri: https://account.radpowerbikes.com/authentication/.well-known/jwks.json
  openIdConnectUrl: https://www.radpowerbikes.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://account.radpowerbikes.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: rad-power-bikes-authentication
source_filename: rad-power-bikes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://www.radpowerbikes.com/.well-known/openid-configuration,\n  https://www.radpowerbikes.com/.well-known/oauth-protected-resource,\n  https://www.radpowerbikes.com/api/ucp/mcp (anonymous tools/list, HTTP 200)\nsummary: >-\n  Two distinct auth postures. The UCP/MCP commerce surface is ANONYMOUS — tools/list and the\n  catalog/cart/checkout tools answered without any credential. Buyer identity, when needed,\n  is carried by an OpenID Connect authorization-code + PKCE flow against Shopify Customer\n  Accounts on the merchant's own account.radpowerbikes.com host. There is no API-key program\n  and no developer key issuance of any kind.\nschemes:\n- id: anonymous-mcp\n  type: none\n  applies_to: https://www.radpowerbikes.com/api/ucp/mcp\n  description: >-\n    The UCP shopping MCP endpoint accepts unauthenticated JSON-RPC. Requests carry a\n    meta.ucp-agent.profile URI identifying the calling agent rather than a bearer\
  \ token.\n    Payment credentials are supplied per-checkout as payment instruments issued by a\n    payment handler (Shop Pay, Shopify card, Google Pay), not as an account credential.\n  evidence:\n    http_status: 200\n    probed: '2026-08-26'\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.radpowerbikes.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7999645\n  authorization_endpoint: https://account.radpowerbikes.com/authentication/oauth/authorize\n  token_endpoint: https://account.radpowerbikes.com/authentication/oauth/token\n  jwks_uri: https://account.radpowerbikes.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.radpowerbikes.com/authentication/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  -\
  \ client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  description: >-\n    Shopify Customer Accounts OIDC, provisioned for shop 7999645 and served from the\n    merchant's own account.radpowerbikes.com host. Client registration is not open to the\n    public; these are the credentials a storefront/app uses on the buyer's behalf.\nprotected_resources:\n- resource: https://www.radpowerbikes.com\n  authorization_servers:\n  - https://account.radpowerbikes.com\n  - https://shopify.com/authentication/7999645\n  bearer_methods_supported:\n  - header\n  rfc: RFC 9728\n- resource: https://account.radpowerbikes.com\n  authorization_servers:\n  - https://account.radpowerbikes.com\n  - https://shopify.com/authentication/7999645\n  bearer_methods_supported:\n  - header\n  rfc: RFC 9728\napi_keys: false\nmtls: false\nnotes:\n- No developer portal, no API key signup, no partner credential program\
  \ was found.\n- >-\n  Checkout completion is gated on human buyer approval by published policy, not by an\n  authentication scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rad-power-bikes/refs/heads/main/authentication/rad-power-bikes-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Electric Bikes
- Micromobility
- Ecommerce
- Retail
- Consumer Products
- Agentic Commerce
- Shopify
- MCP
- Universal Commerce Protocol
---
