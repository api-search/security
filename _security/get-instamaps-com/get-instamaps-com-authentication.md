---
anonymous_access: false
api_key_in: []
api_specs:
- filename: get-instamaps-com-around-a-place-api-openapi.yml
  format: yaml
  label: InstaMaps Around a place API
  slug: get-instamaps-com-around-a-place-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-around-a-place-api-openapi.yml
- filename: get-instamaps-com-ask-a-table-api-openapi.yml
  format: yaml
  label: InstaMaps Ask a table API
  slug: get-instamaps-com-ask-a-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-ask-a-table-api-openapi.yml
- filename: get-instamaps-com-facts-and-risk-api-openapi.yml
  format: yaml
  label: InstaMaps Facts and risk API
  slug: get-instamaps-com-facts-and-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-facts-and-risk-api-openapi.yml
- filename: get-instamaps-com-maps-api-openapi.yml
  format: yaml
  label: InstaMaps Maps API
  slug: get-instamaps-com-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-maps-api-openapi.yml
- filename: get-instamaps-com-measure-api-openapi.yml
  format: yaml
  label: InstaMaps Measure API
  slug: get-instamaps-com-measure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-measure-api-openapi.yml
- filename: get-instamaps-com-place-api-openapi.yml
  format: yaml
  label: InstaMaps Place API
  slug: get-instamaps-com-place-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-place-api-openapi.yml
- filename: get-instamaps-com-route-api-openapi.yml
  format: yaml
  label: InstaMaps Route API
  slug: get-instamaps-com-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-route-api-openapi.yml
- filename: get-instamaps-com-runs-and-jobs-api-openapi.yml
  format: yaml
  label: InstaMaps Runs and jobs API
  slug: get-instamaps-com-runs-and-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/get-instamaps-com/openapi/get-instamaps-com-runs-and-jobs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: InstaMaps Authentication
name_suffix: Authentication
oauth_flows: []
overview: InstaMaps secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InstaMaps
provider_slug: get-instamaps-com
scheme_count: 1
schemes:
- bearerFormat: im_live_…
  description: 'Authorization: Bearer <your API key> (or X-API-Key). Keys are free: sign in with Google at /developers/portal.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/get-instamaps-com-openapi.json
  type: http
slug: get-instamaps-com-authentication
source_filename: get-instamaps-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/get-instamaps-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: im_live_…\n  description: 'Authorization: Bearer <your API key> (or X-API-Key). Keys are free: sign in\n    with Google at /developers/portal.'\n  sources:\n  - openapi/get-instamaps-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/get-instamaps-com/authentication/get-instamaps-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Geocoding
- Mapping
- Route Planning
- Google Sheets Add-on
- Location Data
- Field Service Management
- Sales Territory
---
