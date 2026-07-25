---
api_key_in:
- header
- query
api_specs:
- filename: us-geological-survey-collections-api-openapi.yml
  format: yaml
  label: US Geological Survey Collections API
  slug: us-geological-survey-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-collections-api-openapi.yml
- filename: us-geological-survey-continuous-values-api-openapi.yml
  format: yaml
  label: US Geological Survey Continuous Values API
  slug: us-geological-survey-continuous-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-continuous-values-api-openapi.yml
- filename: us-geological-survey-daily-values-api-openapi.yml
  format: yaml
  label: US Geological Survey Daily Values API
  slug: us-geological-survey-daily-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-daily-values-api-openapi.yml
- filename: us-geological-survey-earthquakes-api-openapi.yml
  format: yaml
  label: US Geological Survey Earthquakes API
  slug: us-geological-survey-earthquakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-earthquakes-api-openapi.yml
- filename: us-geological-survey-field-measurements-api-openapi.yml
  format: yaml
  label: US Geological Survey Field Measurements API
  slug: us-geological-survey-field-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-field-measurements-api-openapi.yml
- filename: us-geological-survey-metadata-api-openapi.yml
  format: yaml
  label: US Geological Survey Metadata API
  slug: us-geological-survey-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-metadata-api-openapi.yml
- filename: us-geological-survey-monitoring-locations-api-openapi.yml
  format: yaml
  label: US Geological Survey Monitoring Locations API
  slug: us-geological-survey-monitoring-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-monitoring-locations-api-openapi.yml
- filename: us-geological-survey-time-series-metadata-api-openapi.yml
  format: yaml
  label: US Geological Survey Time Series Metadata API
  slug: us-geological-survey-time-series-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-time-series-metadata-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Geological Survey Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Geological Survey secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: US Geological Survey
provider_slug: us-geological-survey
scheme_count: 2
schemes:
- description: API key passed as query parameter. Register at https://api.waterdata.usgs.gov/signup/
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/usgs-water-data-openapi.yml
  type: apiKey
- description: API key passed in request header. Register at https://api.waterdata.usgs.gov/signup/
  in: header
  name: ApiKeyHeader
  parameter: api_key
  sources:
  - openapi/usgs-water-data-openapi.yml
  type: apiKey
slug: us-geological-survey-authentication
source_filename: us-geological-survey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usgs-water-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as query parameter. Register at https://api.waterdata.usgs.gov/signup/\n  sources:\n  - openapi/usgs-water-data-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: API key passed in request header. Register at https://api.waterdata.usgs.gov/signup/\n  sources:\n  - openapi/usgs-water-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/authentication/us-geological-survey-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Earth Science
- Earthquakes
- Water Data
- Geospatial
- Hazards
- Environment
---
