---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fanvault-shop-analytics-api-openapi.yml
  format: yaml
  label: fanvault-shop Analytics API
  slug: fanvault-shop-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-analytics-api-openapi.yml
- filename: fanvault-shop-context-api-openapi.yml
  format: yaml
  label: fanvault-shop Context API
  slug: fanvault-shop-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-context-api-openapi.yml
- filename: fanvault-shop-digital-products-api-openapi.yml
  format: yaml
  label: fanvault-shop Digital Products API
  slug: fanvault-shop-digital-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-digital-products-api-openapi.yml
- filename: fanvault-shop-link-in-bio-api-openapi.yml
  format: yaml
  label: fanvault-shop Link in Bio API
  slug: fanvault-shop-link-in-bio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-link-in-bio-api-openapi.yml
- filename: fanvault-shop-listings-api-openapi.yml
  format: yaml
  label: fanvault-shop Listings API
  slug: fanvault-shop-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-listings-api-openapi.yml
- filename: fanvault-shop-media-api-openapi.yml
  format: yaml
  label: fanvault-shop Media API
  slug: fanvault-shop-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-media-api-openapi.yml
- filename: fanvault-shop-messages-api-openapi.yml
  format: yaml
  label: fanvault-shop Messages API
  slug: fanvault-shop-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-messages-api-openapi.yml
- filename: fanvault-shop-orders-api-openapi.yml
  format: yaml
  label: fanvault-shop Orders API
  slug: fanvault-shop-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-orders-api-openapi.yml
- filename: fanvault-shop-payments-api-openapi.yml
  format: yaml
  label: fanvault-shop Payments API
  slug: fanvault-shop-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-payments-api-openapi.yml
- filename: fanvault-shop-posts-api-openapi.yml
  format: yaml
  label: fanvault-shop Posts API
  slug: fanvault-shop-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-posts-api-openapi.yml
- filename: fanvault-shop-profile-api-openapi.yml
  format: yaml
  label: fanvault-shop Profile API
  slug: fanvault-shop-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-profile-api-openapi.yml
- filename: fanvault-shop-scheduling-api-openapi.yml
  format: yaml
  label: fanvault-shop Scheduling API
  slug: fanvault-shop-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-scheduling-api-openapi.yml
- filename: fanvault-shop-social-api-openapi.yml
  format: yaml
  label: fanvault-shop Social API
  slug: fanvault-shop-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-social-api-openapi.yml
- filename: fanvault-shop-wishlist-api-openapi.yml
  format: yaml
  label: fanvault-shop Wishlist API
  slug: fanvault-shop-wishlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanvault-shop/openapi/fanvault-shop-wishlist-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: fanvault-shop Authentication
name_suffix: Authentication
oauth_flows: []
overview: fanvault-shop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: fanvault-shop
provider_slug: fanvault-shop
scheme_count: 1
schemes:
- description: 'A Fanvault personal access token (fv_mcp_…), created at /settings/cli or /settings/mcp, or an OAuth 2.1 access token. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fanvault-shop-openapi.json
  type: http
slug: fanvault-shop-authentication
source_filename: fanvault-shop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fanvault-shop-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Fanvault personal access token (fv_mcp_…), created at /settings/cli or /settings/mcp,\n    or an OAuth 2.1 access token. Sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/fanvault-shop-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fanvault-shop/authentication/fanvault-shop-authentication.yml
summary_line: http · 1 scheme
tags:
- Creator Commerce
- Marketplace
- Payments
- Subscription
- Shipping
---
