---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: travel-risk-api-adb-api-openapi.yml
  format: yaml
  label: Travel Risk API Adb API
  slug: travel-risk-api-adb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-adb-api-openapi.yml
- filename: travel-risk-api-auth-api-openapi.yml
  format: yaml
  label: Travel Risk API Auth API
  slug: travel-risk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-auth-api-openapi.yml
- filename: travel-risk-api-billing-api-openapi.yml
  format: yaml
  label: Travel Risk API Billing API
  slug: travel-risk-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-billing-api-openapi.yml
- filename: travel-risk-api-ext-api-openapi.yml
  format: yaml
  label: Travel Risk API Ext API
  slug: travel-risk-api-ext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-ext-api-openapi.yml
- filename: travel-risk-api-public-data-api-openapi.yml
  format: yaml
  label: Travel Risk API Public Data API
  slug: travel-risk-api-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-public-data-api-openapi.yml
- filename: travel-risk-api-system-api-openapi.yml
  format: yaml
  label: Travel Risk API System API
  slug: travel-risk-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-system-api-openapi.yml
- filename: travel-risk-api-usage-api-openapi.yml
  format: yaml
  label: Travel Risk API Usage API
  slug: travel-risk-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Travel Risk Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Travel Risk API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Travel Risk API
provider_slug: travel-risk-api
scheme_count: 2
schemes:
- description: Your key from https://travelriskapi.com — free plan, no card.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/travel-risk-api-aviation-openapi.yml
  - openapi/travel-risk-api-openapi.yml
  type: apiKey
- description: Same key as a query parameter, for clients that cannot send headers.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/travel-risk-api-aviation-openapi.yml
  type: apiKey
slug: travel-risk-api-authentication
source_filename: travel-risk-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/travel-risk-api-aviation-openapi.yml, openapi/travel-risk-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your key from https://travelriskapi.com — free plan, no card.\n  sources:\n  - openapi/travel-risk-api-aviation-openapi.yml\n  - openapi/travel-risk-api-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Same key as a query parameter, for clients that cannot send headers.\n  sources:\n  - openapi/travel-risk-api-aviation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/authentication/travel-risk-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Travel
- Travel Risk
- Travel Advisories
- Aviation
- Airports
- Risk Scoring
- Safety
- Disaster Alerts
---
