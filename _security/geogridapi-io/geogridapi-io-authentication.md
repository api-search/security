---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geogridapi-io-account-api-openapi.yml
  format: yaml
  label: GeoGridAPI Account API
  slug: geogridapi-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-account-api-openapi.yml
- filename: geogridapi-io-batches-api-openapi.yml
  format: yaml
  label: GeoGridAPI Batches API
  slug: geogridapi-io-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-batches-api-openapi.yml
- filename: geogridapi-io-grids-api-openapi.yml
  format: yaml
  label: GeoGridAPI Grids API
  slug: geogridapi-io-grids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-grids-api-openapi.yml
- filename: geogridapi-io-listings-api-openapi.yml
  format: yaml
  label: GeoGridAPI Listings API
  slug: geogridapi-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-listings-api-openapi.yml
- filename: geogridapi-io-schedules-api-openapi.yml
  format: yaml
  label: GeoGridAPI Schedules API
  slug: geogridapi-io-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-schedules-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GeoGridAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: GeoGridAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GeoGridAPI
provider_slug: geogridapi-io
scheme_count: 1
schemes:
- description: gga_live_… or gga_test_… key from the console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/geogridapi-io-openapi.json
  type: http
slug: geogridapi-io-authentication
source_filename: geogridapi-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/geogridapi-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: gga_live_… or gga_test_… key from the console.\n  sources:\n  - openapi/geogridapi-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/geogridapi-io/authentication/geogridapi-io-authentication.yml
summary_line: http · 1 scheme
tags:
- GeoGridAPI
- Mapping
- SEO
- Business
---
