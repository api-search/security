---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ecmwf-data-stores-processing-openapi.yml
  format: yaml
  label: ECMWF Data Stores Processing API
  slug: ecmwf-data-stores-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-processing-openapi.yml
- filename: ecmwf-data-stores-catalogue-openapi.yml
  format: yaml
  label: ECMWF Data Stores STAC Catalogue API
  slug: ecmwf-data-stores-stac-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-catalogue-openapi.yml
- filename: ecmwf-data-stores-profiles-openapi.yml
  format: yaml
  label: ECMWF Data Stores Profile API
  slug: ecmwf-data-stores-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-profiles-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ecmwf Authentication
name_suffix: Authentication
oauth_flows: []
overview: ECMWF declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ECMWF
provider_slug: ecmwf
scheme_count: 2
schemes:
- description: Personal access token for Climate Data Store API
  docs: https://cds.climate.copernicus.eu/how-to-api
  format: Bearer <token>
  location: header
  name: CDS API
  parameter: Authorization
  type: apiKey
- description: API key for ECMWF Web API (MARS access)
  docs: https://confluence.ecmwf.int/display/WEBAPI
  format: JSON configuration file
  location: config file
  name: ECMWF Web API
  parameter: key
  type: apiKey
slug: ecmwf-authentication
source_filename: ecmwf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://cds.climate.copernicus.eu/how-to-api ; https://confluence.ecmwf.int/display/WEBAPI\nschemes:\n- type: apiKey\n  name: CDS API\n  description: Personal access token for Climate Data Store API\n  location: header\n  parameter: Authorization\n  format: 'Bearer <token>'\n  docs: https://cds.climate.copernicus.eu/how-to-api\n- type: apiKey\n  name: ECMWF Web API\n  description: API key for ECMWF Web API (MARS access)\n  location: config file\n  parameter: key\n  format: JSON configuration file\n  docs: https://confluence.ecmwf.int/display/WEBAPI\nnote: ECMWF uses API keys/tokens for authentication. CDS API uses personal access tokens via Authorization header. ECMWF Web API uses API keys stored in configuration files."
source_yaml_url: https://artifacts.apis.io/ecmwf/authentication/ecmwf-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Weather
- Meteorology
- Forecasting
- Climate
- Open Data
- Research
- Intergovernmental
---
