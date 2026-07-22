---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Urtopia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Urtopia secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Urtopia
provider_slug: urtopia
scheme_count: 2
schemes:
- authorizationUrl: https://shopify.com/authentication/58358104213/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/58358104213
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://newurtopia.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/urtopia-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/58358104213/oauth/token
  type: openIdConnect
- description: Read-only product/collection JSON endpoints and the Storefront MCP tools/list surface require no authentication.
  name: AnonymousStorefrontRead
  sources:
  - llms/urtopia-llms.txt
  type: none
slug: urtopia-authentication
source_filename: urtopia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://newurtopia.com/.well-known/openid-configuration\nnotes: >-\n  Urtopia publishes no proprietary developer API. The authentication surface\n  on newurtopia.com is Shopify Customer Account OIDC (served natively via\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  on the store host). The storefront agent surfaces (Storefront MCP,\n  UCP read-only catalog endpoints) are unauthenticated for read-only browsing;\n  checkout requires buyer-approved payment per the store's llms.txt rules.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  anonymous_read: true\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://newurtopia.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/58358104213\n    authorizationUrl: https://shopify.com/authentication/58358104213/oauth/authorize\n\
  \    tokenUrl: https://shopify.com/authentication/58358104213/oauth/token\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    code_challenge_methods: [S256]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    sources: [well-known/urtopia-openid-configuration.json]\n  - name: AnonymousStorefrontRead\n    type: none\n    description: >-\n      Read-only product/collection JSON endpoints and the Storefront MCP\n      tools/list surface require no authentication.\n    sources: [llms/urtopia-llms.txt]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urtopia/refs/heads/main/authentication/urtopia-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- E-Bikes
- Electric Vehicles
- Cycling
- Smart Hardware
- Mobility
- eCommerce
---
