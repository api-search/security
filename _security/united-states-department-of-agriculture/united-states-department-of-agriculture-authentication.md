---
api_key_in:
- query
api_specs:
- filename: united-states-department-of-agriculture-data-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Data API
  slug: united-states-department-of-agriculture-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-data-api-openapi.yml
- filename: united-states-department-of-agriculture-foods-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Foods API
  slug: united-states-department-of-agriculture-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-foods-api-openapi.yml
- filename: united-states-department-of-agriculture-forecasts-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Forecasts API
  slug: united-states-department-of-agriculture-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-forecasts-api-openapi.yml
- filename: united-states-department-of-agriculture-metadata-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Metadata API
  slug: united-states-department-of-agriculture-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-metadata-api-openapi.yml
- filename: united-states-department-of-agriculture-nutrients-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Nutrients API
  slug: united-states-department-of-agriculture-nutrients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-nutrients-api-openapi.yml
- filename: united-states-department-of-agriculture-stations-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Stations API
  slug: united-states-department-of-agriculture-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-stations-api-openapi.yml
- filename: united-states-department-of-agriculture-statistics-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Statistics API
  slug: united-states-department-of-agriculture-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-statistics-api-openapi.yml
- filename: united-states-department-of-agriculture-survey-data-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Survey Data API
  slug: united-states-department-of-agriculture-survey-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-survey-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: United States Department Of Agriculture Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Department of Agriculture secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: United States Department of Agriculture
provider_slug: united-states-department-of-agriculture
scheme_count: 2
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/usda-ers-arms-openapi.yml
  - openapi/usda-fooddata-central-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/usda-nass-quickstats-openapi.yml
  type: apiKey
slug: united-states-department-of-agriculture-authentication
source_filename: united-states-department-of-agriculture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usda-ers-arms-openapi.yml, openapi/usda-fooddata-central-openapi.yml, openapi/usda-nass-quickstats-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/usda-ers-arms-openapi.yml\n  - openapi/usda-fooddata-central-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/usda-nass-quickstats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/authentication/united-states-department-of-agriculture-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Rural Development
- Climate
---
