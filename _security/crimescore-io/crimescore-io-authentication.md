---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crimescore-io-geocode-api-openapi.yml
  format: yaml
  label: crimescore-io Geocode API
  slug: crimescore-io-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-geocode-api-openapi.yml
- filename: crimescore-io-incidents-api-openapi.yml
  format: yaml
  label: crimescore-io Incidents API
  slug: crimescore-io-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-incidents-api-openapi.yml
- filename: crimescore-io-score-api-openapi.yml
  format: yaml
  label: crimescore-io Score API
  slug: crimescore-io-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-score-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crimescore Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: crimescore-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: crimescore-io
provider_slug: crimescore-io
scheme_count: 1
schemes:
- description: API key required for all requests except public geocode.
  in: header
  name: x-api-key
  type: apiKey
slug: crimescore-io-authentication
source_filename: crimescore-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: \"https://crimescore.io/openapi.yaml\"\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key required for all requests except public geocode.\n"
source_yaml_url: https://artifacts.apis.io/crimescore-io/authentication/crimescore-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Safety
- RealEstate
- Data
- Mapping
- API
---
