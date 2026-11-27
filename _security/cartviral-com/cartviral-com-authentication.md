---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cartviral-com-account-api-openapi.yml
  format: yaml
  label: CartViral Account API
  slug: cartviral-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-account-api-openapi.yml
- filename: cartviral-com-carousels-api-openapi.yml
  format: yaml
  label: CartViral Carousels API
  slug: cartviral-com-carousels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-carousels-api-openapi.yml
- filename: cartviral-com-characters-api-openapi.yml
  format: yaml
  label: CartViral Characters API
  slug: cartviral-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-characters-api-openapi.yml
- filename: cartviral-com-clips-api-openapi.yml
  format: yaml
  label: CartViral Clips API
  slug: cartviral-com-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-clips-api-openapi.yml
- filename: cartviral-com-create-api-openapi.yml
  format: yaml
  label: CartViral Create API
  slug: cartviral-com-create-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-create-api-openapi.yml
- filename: cartviral-com-creations-api-openapi.yml
  format: yaml
  label: CartViral Creations API
  slug: cartviral-com-creations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-creations-api-openapi.yml
- filename: cartviral-com-media-api-openapi.yml
  format: yaml
  label: CartViral Media API
  slug: cartviral-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-media-api-openapi.yml
- filename: cartviral-com-offers-api-openapi.yml
  format: yaml
  label: CartViral Offers API
  slug: cartviral-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-offers-api-openapi.yml
- filename: cartviral-com-photos-api-openapi.yml
  format: yaml
  label: CartViral Photos API
  slug: cartviral-com-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-photos-api-openapi.yml
- filename: cartviral-com-pitches-api-openapi.yml
  format: yaml
  label: CartViral Pitches API
  slug: cartviral-com-pitches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-pitches-api-openapi.yml
- filename: cartviral-com-products-api-openapi.yml
  format: yaml
  label: CartViral Products API
  slug: cartviral-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-products-api-openapi.yml
- filename: cartviral-com-static-ads-api-openapi.yml
  format: yaml
  label: CartViral Static Ads API
  slug: cartviral-com-static-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-static-ads-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: CartViral Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CartViral secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CartViral
provider_slug: cartviral-com
scheme_count: 2
schemes:
- description: API key from Account → AI agents (cv_live_...), or an OAuth access token
  name: bearer
  scheme: bearer
  sources:
  - openapi/cartviral-com-openapi.json
  type: http
- flows:
  - authorizationUrl: https://app.cartviral.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://app.cartviral.com/oauth/token
  name: oauth
  sources:
  - openapi/cartviral-com-openapi.json
  type: oauth2
slug: cartviral-com-authentication
source_filename: cartviral-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/cartviral-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key from Account → AI agents (cv_live_...), or an OAuth access token\n  sources:\n  - openapi/cartviral-com-openapi.json\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.cartviral.com/oauth/authorize\n    tokenUrl: https://app.cartviral.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/cartviral-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cartviral-com/authentication/cartviral-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Video Generation
- Marketing
---
