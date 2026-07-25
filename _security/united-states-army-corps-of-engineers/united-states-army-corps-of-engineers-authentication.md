---
api_key_in: []
api_specs:
- filename: united-states-army-corps-of-engineers-basins-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Basins API
  slug: united-states-army-corps-of-engineers-basins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-basins-api-openapi.yml
- filename: united-states-army-corps-of-engineers-catalog-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Catalog API
  slug: united-states-army-corps-of-engineers-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-catalog-api-openapi.yml
- filename: united-states-army-corps-of-engineers-forecasts-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Forecasts API
  slug: united-states-army-corps-of-engineers-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-forecasts-api-openapi.yml
- filename: united-states-army-corps-of-engineers-levels-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Levels API
  slug: united-states-army-corps-of-engineers-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-levels-api-openapi.yml
- filename: united-states-army-corps-of-engineers-locations-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Locations API
  slug: united-states-army-corps-of-engineers-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-locations-api-openapi.yml
- filename: united-states-army-corps-of-engineers-parameters-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Parameters API
  slug: united-states-army-corps-of-engineers-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-parameters-api-openapi.yml
- filename: united-states-army-corps-of-engineers-projects-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Projects API
  slug: united-states-army-corps-of-engineers-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-projects-api-openapi.yml
- filename: united-states-army-corps-of-engineers-ratings-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Ratings API
  slug: united-states-army-corps-of-engineers-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-ratings-api-openapi.yml
- filename: united-states-army-corps-of-engineers-time-series-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Time Series API
  slug: united-states-army-corps-of-engineers-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-time-series-api-openapi.yml
- filename: united-states-army-corps-of-engineers-version-api-openapi.yml
  format: yaml
  label: United States Army Corps of Engineers Version API
  slug: united-states-army-corps-of-engineers-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/openapi/united-states-army-corps-of-engineers-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: United States Army Corps Of Engineers Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Army Corps of Engineers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United States Army Corps of Engineers
provider_slug: united-states-army-corps-of-engineers
scheme_count: 1
schemes:
- description: JWT Bearer token for authenticated operations (create, update, delete). Obtain a token from the CWMS authorization endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cwms-data-api-openapi.yml
  type: http
slug: united-states-army-corps-of-engineers-authentication
source_filename: united-states-army-corps-of-engineers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cwms-data-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT Bearer token for authenticated operations (create, update, delete). Obtain\n    a token from the CWMS authorization endpoint.\n  sources:\n  - openapi/cwms-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-army-corps-of-engineers/refs/heads/main/authentication/united-states-army-corps-of-engineers-authentication.yml
summary_line: http · 1 scheme
tags:
- Engineering
- Federal Government
- Water Resources
- Hydrology
- Civil Engineering
---
