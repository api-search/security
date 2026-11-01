---
anonymous_access: false
api_key_in: []
api_specs:
- filename: stream-estate-indicators-api-openapi.yml
  format: yaml
  label: stream-estate Indicators API
  slug: stream-estate-indicators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-indicators-api-openapi.yml
- filename: stream-estate-properties-api-openapi.yml
  format: yaml
  label: stream-estate Properties API
  slug: stream-estate-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-properties-api-openapi.yml
- filename: stream-estate-searches-api-openapi.yml
  format: yaml
  label: stream-estate Searches API
  slug: stream-estate-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-searches-api-openapi.yml
- filename: stream-estate-webhooks-api-openapi.yml
  format: yaml
  label: stream-estate Webhooks API
  slug: stream-estate-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Stream Estate Authentication
name_suffix: Authentication
oauth_flows: []
overview: stream-estate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: stream-estate
provider_slug: stream-estate
scheme_count: 1
schemes:
- description: API key required for all requests
  in: header
  name: X-API-KEY
  type: apiKey
slug: stream-estate-authentication
source_filename: stream-estate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/stream-estate-openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-KEY\n    in: header\n    description: \"API key required for all requests\"\n"
source_yaml_url: https://artifacts.apis.io/stream-estate/authentication/stream-estate-authentication.yml
summary_line: 1 scheme
tags:
- RealEstate
- PropTech
- DataAPI
- MarketAnalytics
- Valuation
---
