---
api_key_in: []
api_specs:
- filename: wish-marketplace-v3-openapi.json
  format: json
  label: Wish Marketplace V3 API
  slug: wish-marketplace-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-marketplace-v3-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Wish Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wish secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wish
provider_slug: wish
scheme_count: 2
schemes:
- name: OpenID
  openIdConnectUrl: https://merchant.wish.com/oidc/.well-known/openid-configuration
  sources:
  - openapi/wish-marketplace-v3-openapi.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://merchant.wish.com/v3/oauth/authorize
    flow: authorizationCode
    scopes: 37
    tokenUrl: https://merchant.wish.com/api/v3/oauth/access_token
  name: OAuth2
  sources:
  - openapi/wish-marketplace-v3-openapi.json
  type: oauth2
slug: wish-authentication
source_filename: wish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wish-marketplace-v3-openapi.json\ndocs: https://merchant.wish.com/documentation/api/v3/oauth\nnotes: 'Access tokens are sent as: Authorization: Bearer <token>. OAuth guide at docs URL;\n  OIDC discovery live at https://merchant.wish.com/oidc/.well-known/openid-configuration.'\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OpenID\n  type: openIdConnect\n  openIdConnectUrl: https://merchant.wish.com/oidc/.well-known/openid-configuration\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://merchant.wish.com/v3/oauth/authorize\n    tokenUrl: https://merchant.wish.com/api/v3/oauth/access_token\n    scopes: 37\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/authentication/wish-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Merchants
- Orders
- Products
- Fulfillment
- Shopping
- OAuth
---
