---
anonymous_access: false
api_key_in: []
api_specs:
- filename: transcapi-airports-api-openapi.yml
  format: yaml
  label: TransCAPI Airports API
  slug: transcapi-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-airports-api-openapi.yml
- filename: transcapi-alerts-api-openapi.yml
  format: yaml
  label: TransCAPI Alerts API
  slug: transcapi-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-alerts-api-openapi.yml
- filename: transcapi-bus-api-openapi.yml
  format: yaml
  label: TransCAPI Bus API
  slug: transcapi-bus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-bus-api-openapi.yml
- filename: transcapi-disruptions-api-openapi.yml
  format: yaml
  label: TransCAPI Disruptions API
  slug: transcapi-disruptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-disruptions-api-openapi.yml
- filename: transcapi-journey-api-openapi.yml
  format: yaml
  label: TransCAPI Journey API
  slug: transcapi-journey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-journey-api-openapi.yml
- filename: transcapi-places-api-openapi.yml
  format: yaml
  label: TransCAPI Places API
  slug: transcapi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-places-api-openapi.yml
- filename: transcapi-rail-api-openapi.yml
  format: yaml
  label: TransCAPI Rail API
  slug: transcapi-rail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-rail-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Transcapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: TransCAPI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TransCAPI
provider_slug: transcapi
scheme_count: 2
schemes:
- description: API key passed in header
  in: header
  name: X-Api-Key
  type: apiKey
- description: API key passed as query parameter
  in: query
  name: api_key
  type: apiKey
slug: transcapi-authentication
source_filename: transcapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://api.transcapi.com/openapi.json\nschemes:\n  - type: apiKey\n    in: header\n    name: X-Api-Key\n    description: API key passed in header\n  - type: apiKey\n    in: query\n    name: api_key\n    description: API key passed as query parameter\n"
source_yaml_url: https://artifacts.apis.io/transcapi/authentication/transcapi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Transport
- API
- UK
- Ireland
---
