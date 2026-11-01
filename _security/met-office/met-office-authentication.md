---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: met-office-capabilities-api-openapi.yml
  format: yaml
  label: Met Office Capabilities API
  slug: met-office-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-capabilities-api-openapi.yml
- filename: met-office-collection-metadata-api-openapi.yml
  format: yaml
  label: Met Office Collection Metadata API
  slug: met-office-collection-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-collection-metadata-api-openapi.yml
- filename: met-office-instance-data-api-openapi.yml
  format: yaml
  label: Met Office Instance Data API
  slug: met-office-instance-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-data-api-openapi.yml
- filename: met-office-instance-metadata-api-openapi.yml
  format: yaml
  label: Met Office Instance Metadata API
  slug: met-office-instance-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-metadata-api-openapi.yml
- filename: met-office-met-office-land-observations-public-api-api-openapi.yml
  format: yaml
  label: Met Office Met Office Land Observations Public API
  slug: met-office-met-office-land-observations-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-met-office-land-observations-public-api-api-openapi.yml
- filename: met-office-nearest-api-openapi.yml
  format: yaml
  label: Met Office Nearest API
  slug: met-office-nearest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-nearest-api-openapi.yml
- filename: met-office-objects-api-openapi.yml
  format: yaml
  label: Met Office Objects API
  slug: met-office-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-objects-api-openapi.yml
- filename: met-office-orders-api-openapi.yml
  format: yaml
  label: Met Office Orders API
  slug: met-office-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-orders-api-openapi.yml
- filename: met-office-point-api-openapi.yml
  format: yaml
  label: Met Office Point API
  slug: met-office-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-point-api-openapi.yml
- filename: met-office-runs-api-openapi.yml
  format: yaml
  label: Met Office Runs API
  slug: met-office-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-runs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Met Office Authentication
name_suffix: Authentication
oauth_flows: []
overview: Met Office secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Met Office
provider_slug: met-office
scheme_count: 1
schemes:
- description: The API Key generated with your Subscription in Weather DataHub, this must be set as 'apikey' in your header.
  in: header
  name: APIKey
  parameter: apikey
  sources:
  - openapi/met-office-atmospheric-models-openapi.yml
  - openapi/met-office-blended-probabilistic-forecast-openapi.yml
  - openapi/met-office-land-observations-openapi.yml
  - openapi/met-office-map-images-openapi.yml
  - openapi/met-office-nswws-warnings-openapi.yml
  - openapi/met-office-site-specific-openapi.yml
  type: apiKey
slug: met-office-authentication
source_filename: met-office-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://datahub.metoffice.gov.uk/docs/getting-started\ndocs: https://datahub.metoffice.gov.uk/docs/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: The API Key generated with your Subscription in Weather DataHub, this must be\n    set as 'apikey' in your header.\n  sources:\n  - openapi/met-office-atmospheric-models-openapi.yml\n  - openapi/met-office-blended-probabilistic-forecast-openapi.yml\n  - openapi/met-office-land-observations-openapi.yml\n  - openapi/met-office-map-images-openapi.yml\n  - openapi/met-office-nswws-warnings-openapi.yml\n  - openapi/met-office-site-specific-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/met-office/authentication/met-office-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Weather
- Climate
- Forecast
- Meteorology
- Government
- Open Data
- United Kingdom
---
