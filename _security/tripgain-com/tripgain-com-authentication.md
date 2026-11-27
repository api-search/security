---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tripgain-com-aggregate-api-openapi.yml
  format: yaml
  label: TripGain Aggregate API
  slug: tripgain-com-aggregate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-aggregate-api-openapi.yml
- filename: tripgain-com-analytics-api-openapi.yml
  format: yaml
  label: TripGain Analytics API
  slug: tripgain-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-analytics-api-openapi.yml
- filename: tripgain-com-auth-api-openapi.yml
  format: yaml
  label: TripGain Auth API
  slug: tripgain-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-auth-api-openapi.yml
- filename: tripgain-com-config-api-openapi.yml
  format: yaml
  label: TripGain Config API
  slug: tripgain-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-config-api-openapi.yml
- filename: tripgain-com-flight-analytics-api-api-openapi.yml
  format: yaml
  label: TripGain Flight Analytics API
  slug: tripgain-com-flight-analytics-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-flight-analytics-api-api-openapi.yml
- filename: tripgain-com-flight-search-api-openapi.yml
  format: yaml
  label: TripGain Flight Search API
  slug: tripgain-com-flight-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-flight-search-api-openapi.yml
- filename: tripgain-com-gateway-request-analytics-api-openapi.yml
  format: yaml
  label: TripGain Gateway Request Analytics API
  slug: tripgain-com-gateway-request-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gateway-request-analytics-api-openapi.yml
- filename: tripgain-com-gateway-response-analytics-api-openapi.yml
  format: yaml
  label: TripGain Gateway Response Analytics API
  slug: tripgain-com-gateway-response-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gateway-response-analytics-api-openapi.yml
- filename: tripgain-com-gatewaylog-api-openapi.yml
  format: yaml
  label: TripGain Gateway Log API
  slug: tripgain-com-gatewaylog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gatewaylog-api-openapi.yml
- filename: tripgain-com-hotel-search-api-openapi.yml
  format: yaml
  label: TripGain Hotel Search API
  slug: tripgain-com-hotel-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-hotel-search-api-openapi.yml
- filename: tripgain-com-ingest-batch-api-openapi.yml
  format: yaml
  label: TripGain Ingest Batch API
  slug: tripgain-com-ingest-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-batch-api-openapi.yml
- filename: tripgain-com-ingest-hotel-batch-api-openapi.yml
  format: yaml
  label: TripGain Ingest Hotel Batch API
  slug: tripgain-com-ingest-hotel-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-hotel-batch-api-openapi.yml
- filename: tripgain-com-ingest-hotel-single-api-openapi.yml
  format: yaml
  label: TripGain Ingest Hotel Single API
  slug: tripgain-com-ingest-hotel-single-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-hotel-single-api-openapi.yml
- filename: tripgain-com-ingest-single-api-openapi.yml
  format: yaml
  label: TripGain Ingest Single API
  slug: tripgain-com-ingest-single-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-single-api-openapi.yml
- filename: tripgain-com-stats-api-openapi.yml
  format: yaml
  label: TripGain Stats API
  slug: tripgain-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-stats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: TripGain Authentication
name_suffix: Authentication
oauth_flows: []
overview: TripGain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TripGain
provider_slug: tripgain-com
scheme_count: 1
schemes:
- in: header
  name: SessionToken
  parameter: x-session-token
  sources:
  - openapi/tripgain-com-openapi.json
  type: apiKey
slug: tripgain-com-authentication
source_filename: tripgain-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: derived\nsource: openapi/tripgain-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: x-session-token\n  sources:\n  - openapi/tripgain-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tripgain-com/authentication/tripgain-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel
- AI
- Corporate
- ExpenseManagement
- Software
---
