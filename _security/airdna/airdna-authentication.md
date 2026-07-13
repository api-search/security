---
api_key_in: []
api_specs:
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Search
  slug: market-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Stats
  slug: market-stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Property/Listing Data
  slug: property-listing-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Estimates
  slug: rentalizer-estimates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Comps
  slug: comps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/authentication/airdna-authentication.yml
summary_line: http · 1 scheme
tags:
- Short-Term Rental
- Vacation Rental
- Market Data
- Real Estate
- Analytics
---
