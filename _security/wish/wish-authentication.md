---
api_key_in: []
api_specs:
- filename: wish-brands-api-openapi.yml
  format: yaml
  label: Wish Brands API
  slug: wish-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-brands-api-openapi.yml
- filename: wish-bulk-products-api-openapi.yml
  format: yaml
  label: Wish Bulk Products API
  slug: wish-bulk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-bulk-products-api-openapi.yml
- filename: wish-currencies-api-openapi.yml
  format: yaml
  label: Wish Currencies API
  slug: wish-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-currencies-api-openapi.yml
- filename: wish-eu-product-compliance-api-openapi.yml
  format: yaml
  label: Wish EU Product Compliance API
  slug: wish-eu-product-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-eu-product-compliance-api-openapi.yml
- filename: wish-france-epr-compliance-api-openapi.yml
  format: yaml
  label: Wish France EPR Compliance API
  slug: wish-france-epr-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-france-epr-compliance-api-openapi.yml
- filename: wish-germany-epr-compliance-api-openapi.yml
  format: yaml
  label: Wish Germany EPR Compliance API
  slug: wish-germany-epr-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-germany-epr-compliance-api-openapi.yml
- filename: wish-merchant-api-openapi.yml
  format: yaml
  label: Wish Merchant API
  slug: wish-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-merchant-api-openapi.yml
- filename: wish-oauth-api-openapi.yml
  format: yaml
  label: Wish OAuth API
  slug: wish-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-oauth-api-openapi.yml
- filename: wish-orders-api-openapi.yml
  format: yaml
  label: Wish Orders API
  slug: wish-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-orders-api-openapi.yml
- filename: wish-payments-api-openapi.yml
  format: yaml
  label: Wish Payments API
  slug: wish-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-payments-api-openapi.yml
- filename: wish-penalties-api-openapi.yml
  format: yaml
  label: Wish Penalties API
  slug: wish-penalties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-penalties-api-openapi.yml
- filename: wish-productboost-api-openapi.yml
  format: yaml
  label: Wish ProductBoost API
  slug: wish-productboost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-productboost-api-openapi.yml
- filename: wish-products-api-openapi.yml
  format: yaml
  label: Wish Products API
  slug: wish-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-products-api-openapi.yml
- filename: wish-promotions-platform-api-openapi.yml
  format: yaml
  label: Wish Promotions Platform API
  slug: wish-promotions-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-promotions-platform-api-openapi.yml
- filename: wish-ratings-api-openapi.yml
  format: yaml
  label: Wish Ratings API
  slug: wish-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-ratings-api-openapi.yml
- filename: wish-taxonomy-api-openapi.yml
  format: yaml
  label: Wish Taxonomy API
  slug: wish-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-taxonomy-api-openapi.yml
- filename: wish-tickets-api-openapi.yml
  format: yaml
  label: Wish Tickets API
  slug: wish-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-tickets-api-openapi.yml
- filename: wish-unification-initiative-api-openapi.yml
  format: yaml
  label: Wish Unification Initiative API
  slug: wish-unification-initiative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-unification-initiative-api-openapi.yml
- filename: wish-variations-api-openapi.yml
  format: yaml
  label: Wish Variations API
  slug: wish-variations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-variations-api-openapi.yml
- filename: wish-videos-api-openapi.yml
  format: yaml
  label: Wish Videos API
  slug: wish-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-videos-api-openapi.yml
- filename: wish-webhook-api-openapi.yml
  format: yaml
  label: Wish Webhook API
  slug: wish-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-webhook-api-openapi.yml
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
