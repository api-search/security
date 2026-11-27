---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: megaphone-campaigns-api-openapi.yml
  format: yaml
  label: Megaphone Campaigns API
  slug: megaphone-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-campaigns-api-openapi.yml
- filename: megaphone-direct-sales-v2-api-openapi.yml
  format: yaml
  label: Megaphone Direct Sales v2 API
  slug: megaphone-direct-sales-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-direct-sales-v2-api-openapi.yml
- filename: megaphone-episodes-api-openapi.yml
  format: yaml
  label: Megaphone Episodes API
  slug: megaphone-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-episodes-api-openapi.yml
- filename: megaphone-exports-api-openapi.yml
  format: yaml
  label: Megaphone Exports API
  slug: megaphone-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-exports-api-openapi.yml
- filename: megaphone-networks-api-openapi.yml
  format: yaml
  label: Megaphone Networks API
  slug: megaphone-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-networks-api-openapi.yml
- filename: megaphone-orders-api-openapi.yml
  format: yaml
  label: Megaphone Orders API
  slug: megaphone-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-orders-api-openapi.yml
- filename: megaphone-podcasts-api-openapi.yml
  format: yaml
  label: Megaphone Podcasts API
  slug: megaphone-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-podcasts-api-openapi.yml
- filename: megaphone-advertisements-api-openapi.yml
  format: yaml
  label: Megaphone Advertisements API
  slug: megaphone-advertisements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-advertisements-api-openapi.yml
- filename: megaphone-advertiser-categories-api-openapi.yml
  format: yaml
  label: Megaphone Advertiser Categories API
  slug: megaphone-advertiser-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-advertiser-categories-api-openapi.yml
- filename: megaphone-advertisers-api-openapi.yml
  format: yaml
  label: Megaphone Advertisers API
  slug: megaphone-advertisers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-advertisers-api-openapi.yml
- filename: megaphone-agencies-api-openapi.yml
  format: yaml
  label: Megaphone Agencies API
  slug: megaphone-agencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-agencies-api-openapi.yml
- filename: megaphone-campaign-orders-api-openapi.yml
  format: yaml
  label: Megaphone Campaign Orders API
  slug: megaphone-campaign-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-campaign-orders-api-openapi.yml
- filename: megaphone-cuepoints-api-openapi.yml
  format: yaml
  label: Megaphone Cuepoints API
  slug: megaphone-cuepoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-cuepoints-api-openapi.yml
- filename: megaphone-direct-sales-api-v2-api-openapi.yml
  format: yaml
  label: Megaphone Direct Sales API v2 API
  slug: megaphone-direct-sales-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-direct-sales-api-v2-api-openapi.yml
- filename: megaphone-iab-advertiser-categories-api-openapi.yml
  format: yaml
  label: Megaphone IAB Advertiser Categories API
  slug: megaphone-iab-advertiser-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-iab-advertiser-categories-api-openapi.yml
- filename: megaphone-organization-tags-api-openapi.yml
  format: yaml
  label: Megaphone Organization Tags API
  slug: megaphone-organization-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-organization-tags-api-openapi.yml
- filename: megaphone-promo-api-v2-api-openapi.yml
  format: yaml
  label: Megaphone Promo API v2 API
  slug: megaphone-promo-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-promo-api-v2-api-openapi.yml
- filename: megaphone-promo-orders-api-openapi.yml
  format: yaml
  label: Megaphone Promo Orders API
  slug: megaphone-promo-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-promo-orders-api-openapi.yml
- filename: megaphone-search-endpoints-api-openapi.yml
  format: yaml
  label: Megaphone Search Endpoints API
  slug: megaphone-search-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-search-endpoints-api-openapi.yml
- filename: megaphone-sponsorships-api-openapi.yml
  format: yaml
  label: Megaphone Sponsorships API
  slug: megaphone-sponsorships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-sponsorships-api-openapi.yml
- filename: megaphone-targeting-api-openapi.yml
  format: yaml
  label: Megaphone Targeting API
  slug: megaphone-targeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/megaphone/openapi/megaphone-targeting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Megaphone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Megaphone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Megaphone
provider_slug: megaphone
scheme_count: 1
schemes:
- description: 'Per-user API token sent as `Authorization: Token token="<API_TOKEN>"`. Generated on account creation and managed under User Settings; treat as a password and do not reuse across organizations.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/megaphone-openapi.yml
  type: apiKey
slug: megaphone-authentication
source_filename: megaphone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/megaphone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Per-user API token sent as `Authorization: Token token=\"<API_TOKEN>\"`. Generated\n    on account creation and managed under User Settings; treat as a password and do not reuse\n    across organizations.'\n  sources:\n  - openapi/megaphone-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/megaphone/authentication/megaphone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasts
- Podcast Hosting
- Advertising
- Ad Monetization
- Dynamic Ad Insertion
- Media
- Spotify
---
