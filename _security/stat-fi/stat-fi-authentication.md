---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: stat-fi-calendar-api-openapi.yml
  format: yaml
  label: Statistics Finland Calendar API
  slug: stat-fi-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-calendar-api-openapi.yml
- filename: stat-fi-capabilities-api-openapi.yml
  format: yaml
  label: Statistics Finland Capabilities API
  slug: stat-fi-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-capabilities-api-openapi.yml
- filename: stat-fi-classificationfamilies-api-openapi.yml
  format: yaml
  label: Statistics Finland Classification Families API
  slug: stat-fi-classificationfamilies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-classificationfamilies-api-openapi.yml
- filename: stat-fi-classifications-api-openapi.yml
  format: yaml
  label: Statistics Finland Classifications API
  slug: stat-fi-classifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-classifications-api-openapi.yml
- filename: stat-fi-classificationseries-api-openapi.yml
  format: yaml
  label: Statistics Finland Classification Series API
  slug: stat-fi-classificationseries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-classificationseries-api-openapi.yml
- filename: stat-fi-correspondencetables-api-openapi.yml
  format: yaml
  label: Statistics Finland Correspondence Tables API
  slug: stat-fi-correspondencetables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-correspondencetables-api-openapi.yml
- filename: stat-fi-current-api-openapi.yml
  format: yaml
  label: Statistics Finland Current API
  slug: stat-fi-current-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-current-api-openapi.yml
- filename: stat-fi-data-api-openapi.yml
  format: yaml
  label: Statistics Finland Data API
  slug: stat-fi-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-data-api-openapi.yml
- filename: stat-fi-databases-api-openapi.yml
  format: yaml
  label: Statistics Finland Databases API
  slug: stat-fi-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-databases-api-openapi.yml
- filename: stat-fi-features-api-openapi.yml
  format: yaml
  label: Statistics Finland Features API
  slug: stat-fi-features-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-features-api-openapi.yml
- filename: stat-fi-metadata-api-openapi.yml
  format: yaml
  label: Statistics Finland Metadata API
  slug: stat-fi-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-metadata-api-openapi.yml
- filename: stat-fi-publications-api-openapi.yml
  format: yaml
  label: Statistics Finland Publications API
  slug: stat-fi-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-publications-api-openapi.yml
- filename: stat-fi-repairstate-api-openapi.yml
  format: yaml
  label: Statistics Finland Repair State API
  slug: stat-fi-repairstate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-repairstate-api-openapi.yml
- filename: stat-fi-search-api-openapi.yml
  format: yaml
  label: Statistics Finland Search API
  slug: stat-fi-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-search-api-openapi.yml
- filename: stat-fi-tables-api-openapi.yml
  format: yaml
  label: Statistics Finland Tables API
  slug: stat-fi-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-fi/openapi/stat-fi-tables-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Statistics Finland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Statistics Finland secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Statistics Finland
provider_slug: stat-fi
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/stat-fi-classifications-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/stat-fi-classifications-openapi.yml
  type: apiKey
slug: stat-fi-authentication
source_filename: stat-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/stat-fi-classifications-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/stat-fi-classifications-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/stat-fi-classifications-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/stat-fi/authentication/stat-fi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Government
- Statistics
- Open Data
- Finland
- Geospatial
- OGC
- PxWeb
---
