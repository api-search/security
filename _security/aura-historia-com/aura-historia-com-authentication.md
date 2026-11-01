---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aura-historia-com-administration-api-openapi.yml
  format: yaml
  label: Aura Historia Administration API
  slug: aura-historia-com-administration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-administration-api-openapi.yml
- filename: aura-historia-com-auctions-api-openapi.yml
  format: yaml
  label: Aura Historia Auctions API
  slug: aura-historia-com-auctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-auctions-api-openapi.yml
- filename: aura-historia-com-billing-api-openapi.yml
  format: yaml
  label: Aura Historia Billing API
  slug: aura-historia-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-billing-api-openapi.yml
- filename: aura-historia-com-listingsources-api-openapi.yml
  format: yaml
  label: Aura Historia Listing Sources API
  slug: aura-historia-com-listingsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-listingsources-api-openapi.yml
- filename: aura-historia-com-newsletter-api-openapi.yml
  format: yaml
  label: Aura Historia Newsletter API
  slug: aura-historia-com-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-newsletter-api-openapi.yml
- filename: aura-historia-com-notifications-api-openapi.yml
  format: yaml
  label: Aura Historia Notifications API
  slug: aura-historia-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-notifications-api-openapi.yml
- filename: aura-historia-com-oauth-api-openapi.yml
  format: yaml
  label: Aura Historia OAuth API
  slug: aura-historia-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-oauth-api-openapi.yml
- filename: aura-historia-com-operations-api-openapi.yml
  format: yaml
  label: Aura Historia Operations API
  slug: aura-historia-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-operations-api-openapi.yml
- filename: aura-historia-com-overview-api-openapi.yml
  format: yaml
  label: Aura Historia Overview API
  slug: aura-historia-com-overview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-overview-api-openapi.yml
- filename: aura-historia-com-parties-api-openapi.yml
  format: yaml
  label: Aura Historia Parties API
  slug: aura-historia-com-parties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-parties-api-openapi.yml
- filename: aura-historia-com-partnershipapplications-api-openapi.yml
  format: yaml
  label: Aura Historia Partnership Applications API
  slug: aura-historia-com-partnershipapplications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-partnershipapplications-api-openapi.yml
- filename: aura-historia-com-partnerships-api-openapi.yml
  format: yaml
  label: Aura Historia Partnerships API
  slug: aura-historia-com-partnerships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-partnerships-api-openapi.yml
- filename: aura-historia-com-party-api-openapi.yml
  format: yaml
  label: Aura Historia Party API
  slug: aura-historia-com-party-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-party-api-openapi.yml
- filename: aura-historia-com-productlistings-api-openapi.yml
  format: yaml
  label: Aura Historia Product Listings API
  slug: aura-historia-com-productlistings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-productlistings-api-openapi.yml
- filename: aura-historia-com-search-filters-api-openapi.yml
  format: yaml
  label: Aura Historia Search Filters API
  slug: aura-historia-com-search-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-search-filters-api-openapi.yml
- filename: aura-historia-com-user-account-api-openapi.yml
  format: yaml
  label: Aura Historia User Account API
  slug: aura-historia-com-user-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-user-account-api-openapi.yml
- filename: aura-historia-com-users-api-openapi.yml
  format: yaml
  label: Aura Historia Users API
  slug: aura-historia-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-users-api-openapi.yml
- filename: aura-historia-com-watchlist-api-openapi.yml
  format: yaml
  label: Aura Historia Watchlist API
  slug: aura-historia-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-watchlist-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Aura Historia Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aura Historia declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aura Historia
provider_slug: aura-historia-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Cognito access JWT bearer token
  name: BearerAuth
  scheme: bearer
  type: http
- bearerFormat: opaque
  description: Aura Historia opaque bearer access token
  name: AccessTokenAuth
  scheme: bearer
  type: http
slug: aura-historia-com-authentication
source_filename: aura-historia-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/aura-historia-com-openapi.yml\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    name: BearerAuth\n    description: Cognito access JWT bearer token\n  - type: http\n    scheme: bearer\n    bearerFormat: opaque\n    name: AccessTokenAuth\n    description: Aura Historia opaque bearer access token\n"
source_yaml_url: https://artifacts.apis.io/aura-historia-com/authentication/aura-historia-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Antiques
- Marketplace
- Search
- SaaS
---
