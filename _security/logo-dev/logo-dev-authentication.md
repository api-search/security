---
anonymous_access: false
api_key_in: []
api_specs:
- filename: logo-dev-account-api-openapi.yml
  format: yaml
  label: Logo.dev Account API
  slug: logo-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-account-api-openapi.yml
- filename: logo-dev-brands-api-openapi.yml
  format: yaml
  label: Logo.dev Brands API
  slug: logo-dev-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-brands-api-openapi.yml
- filename: logo-dev-flags-api-openapi.yml
  format: yaml
  label: Logo.dev Flags API
  slug: logo-dev-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-flags-api-openapi.yml
- filename: logo-dev-logo-cdn-api-openapi.yml
  format: yaml
  label: Logo.dev Logo CDN API
  slug: logo-dev-logo-cdn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logo-cdn-api-openapi.yml
- filename: logo-dev-logos-api-openapi.yml
  format: yaml
  label: Logo.dev Logos API
  slug: logo-dev-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logos-api-openapi.yml
- filename: logo-dev-search-api-openapi.yml
  format: yaml
  label: Logo.dev Search API
  slug: logo-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-search-api-openapi.yml
- filename: logo-dev-subscriptions-api-openapi.yml
  format: yaml
  label: Logo.dev Subscriptions API
  slug: logo-dev-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-subscriptions-api-openapi.yml
- filename: logo-dev-transaction-enrichment-api-api-openapi.yml
  format: yaml
  label: Logo.dev Transaction Enrichment API
  slug: logo-dev-transaction-enrichment-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-transaction-enrichment-api-api-openapi.yml
- filename: logo-dev-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Logo.dev Webhook endpoints API
  slug: logo-dev-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-webhook-endpoints-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Logo.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Logo.dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Logo.dev
provider_slug: logo-dev
scheme_count: 2
schemes:
- description: Publishable key for CDN requests.
  in: query
  name: token
  type: apiKey
- description: Secret key for API requests.
  scheme: bearer
  type: http
slug: logo-dev-authentication
source_filename: logo-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://www.logo.dev/docs/platform/api-keys\nschemes:\n  - type: apiKey\n    in: query\n    name: token\n    description: Publishable key for CDN requests.\n  - type: http\n    scheme: bearer\n    description: Secret key for API requests.\n"
source_yaml_url: https://artifacts.apis.io/logo-dev/authentication/logo-dev-authentication.yml
summary_line: 2 schemes
tags:
- Logo
- Branding
- CDN
- Free Tier
---
