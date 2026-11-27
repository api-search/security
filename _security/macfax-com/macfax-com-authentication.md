---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: macfax-com-alerts-api-openapi.yml
  format: yaml
  label: Macfax Alerts API
  slug: macfax-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-alerts-api-openapi.yml
- filename: macfax-com-briefs-api-openapi.yml
  format: yaml
  label: Macfax Briefs API
  slug: macfax-com-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-briefs-api-openapi.yml
- filename: macfax-com-check-listing-api-openapi.yml
  format: yaml
  label: Macfax Check Listing API
  slug: macfax-com-check-listing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-check-listing-api-openapi.yml
- filename: macfax-com-configs-api-openapi.yml
  format: yaml
  label: Macfax Configs API
  slug: macfax-com-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-configs-api-openapi.yml
- filename: macfax-com-keys-api-openapi.yml
  format: yaml
  label: Macfax Keys API
  slug: macfax-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-keys-api-openapi.yml
- filename: macfax-com-limits-api-openapi.yml
  format: yaml
  label: Macfax Limits API
  slug: macfax-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-limits-api-openapi.yml
- filename: macfax-com-listings-api-openapi.yml
  format: yaml
  label: Macfax Listings API
  slug: macfax-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-listings-api-openapi.yml
- filename: macfax-com-lookup-api-openapi.yml
  format: yaml
  label: Macfax Lookup API
  slug: macfax-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-lookup-api-openapi.yml
- filename: macfax-com-market-api-openapi.yml
  format: yaml
  label: Macfax Market API
  slug: macfax-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-market-api-openapi.yml
- filename: macfax-com-price-stats-api-openapi.yml
  format: yaml
  label: Macfax Price Stats API
  slug: macfax-com-price-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-price-stats-api-openapi.yml
- filename: macfax-com-reports-api-openapi.yml
  format: yaml
  label: Macfax Reports API
  slug: macfax-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/macfax-com/openapi/macfax-com-reports-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Macfax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macfax secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Macfax
provider_slug: macfax-com
scheme_count: 3
schemes:
- description: Optional free API key (mfx_…).
  name: bearer
  scheme: bearer
  sources:
  - openapi/macfax-com-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/macfax-com-openapi.json
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/macfax-com-openapi.json
  type: apiKey
slug: macfax-com-authentication
source_filename: macfax-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/macfax-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Optional free API key (mfx_…).\n  sources:\n  - openapi/macfax-com-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/macfax-com-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/macfax-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/macfax-com/authentication/macfax-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Apple
- SerialLookup
- DeviceVerification
- Marketplace
- E-Commerce
---
