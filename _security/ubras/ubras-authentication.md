---
api_key_in: []
auth_types:
- openIdConnect
description: Authentication profile of Ubras's machine-facing surface, captured from the live discovery documents on ubras.com (the international Shopify storefront). Customer identity uses Shopify customer accounts OIDC (issuer https://shopify.com/authentication/52594442401), published at both /.well-known/openid-configuration and /.well-known/oauth-authorization-server (identical documents, saved in well-known/). The storefront MCP endpoint (/api/mcp) and the read-only product JSON endpoints are anonymous; the UCP shopping MCP (/api/ucp/mcp) requires a UCP agent profile rather than an API key. Ubras publishes no separate first-party developer API keys or OAuth program of its own.
kind: authentication
layout: security
method: searched
name: Ubras Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ubras secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ubras
provider_slug: ubras
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/52594442401/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/52594442401
  jwks_uri: https://shopify.com/authentication/52594442401/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://ubras.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/ubras-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/52594442401/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: ubras-authentication
source_filename: ubras-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://ubras.com/.well-known/openid-configuration\ndescription: >-\n  Authentication profile of Ubras's machine-facing surface, captured from the\n  live discovery documents on ubras.com (the international Shopify\n  storefront). Customer identity uses Shopify customer accounts OIDC (issuer\n  https://shopify.com/authentication/52594442401), published at both\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  (identical documents, saved in well-known/). The storefront MCP endpoint\n  (/api/mcp) and the read-only product JSON endpoints are anonymous; the UCP\n  shopping MCP (/api/ucp/mcp) requires a UCP agent profile rather than an API\n  key. Ubras publishes no separate first-party developer API keys or OAuth\n  program of its own.\nsummary:\n  types: [openIdConnect]\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces:\n    - https://ubras.com/api/mcp (storefront MCP, tools/list unauthenticated)\n\
  \    - https://ubras.com/products/{handle}.json (read-only product JSON)\nschemes:\n  - name: shopify-customer-accounts-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://ubras.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/52594442401\n    authorizationUrl: https://shopify.com/authentication/52594442401/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/52594442401/oauth/token\n    jwks_uri: https://shopify.com/authentication/52594442401/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic]\n    pkce: [S256]\n    scopes_supported:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources: [well-known/ubras-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubras/refs/heads/main/authentication/ubras-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Retail
- eCommerce
- Apparel
- Intimate Apparel
- Direct-to-Consumer
- Agentic Commerce
---
