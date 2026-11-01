---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airdna-market-data-api-openapi.yml
  format: yaml
  label: AirDNA Market Data API
  slug: airdna-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-market-data-api-openapi.yml
- filename: airdna-smart-rates-api-openapi.yml
  format: yaml
  label: AirDNA Smart Rates API
  slug: airdna-smart-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-smart-rates-api-openapi.yml
- filename: airdna-listing-data-api-openapi.yml
  format: yaml
  label: AirDNA Listing Data API
  slug: airdna-listing-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-listing-data-api-openapi.yml
- filename: airdna-rentalizer-data-api-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Data API
  slug: airdna-rentalizer-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-rentalizer-data-api-openapi.yml
- filename: airdna-rentalizer-summary-data-api-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Summary Data API
  slug: airdna-rentalizer-summary-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-rentalizer-summary-data-api-openapi.yml
- filename: airdna-submarket-data-api-openapi.yml
  format: yaml
  label: AirDNA Submarket Data API
  slug: airdna-submarket-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airdna/openapi/airdna-submarket-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Airdna Authentication
name_suffix: Authentication
oauth_flows: []
overview: AirDNA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AirDNA
provider_slug: airdna
scheme_count: 1
schemes:
- description: 'Bearer token supplied in the Authorization header (Authorization: Bearer {API_KEY}). API keys are obtained from AirDNA sales at api@airdna.co.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/airdna-openapi.yml
  type: http
slug: airdna-authentication
source_filename: airdna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airdna-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token supplied in the Authorization header (Authorization: Bearer {API_KEY}).\n    API keys are obtained from AirDNA sales at api@airdna.co.'\n  sources:\n  - openapi/airdna-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/airdna/authentication/airdna-authentication.yml
summary_line: http · 1 scheme
tags:
- Short-Term Rental
- Vacation Rentals
- Market Data
- Real Estate
- Analytics
---
