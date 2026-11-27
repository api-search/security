---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tesseralytics-dev-catalog-api-openapi.yml
  format: yaml
  label: Tessera Analytics Catalog API
  slug: tesseralytics-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tesseralytics-dev/openapi/tesseralytics-dev-catalog-api-openapi.yml
- filename: tesseralytics-dev-datasets-api-openapi.yml
  format: yaml
  label: Tessera Analytics Datasets API
  slug: tesseralytics-dev-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tesseralytics-dev/openapi/tesseralytics-dev-datasets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tessera Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessera Analytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tessera Analytics
provider_slug: tesseralytics-dev
scheme_count: 1
schemes:
- description: Raw API key sent as a bearer token.
  name: api_key
  scheme: bearer
  sources:
  - openapi/tesseralytics-dev-openapi.json
  type: http
slug: tesseralytics-dev-authentication
source_filename: tesseralytics-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/tesseralytics-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  description: Raw API key sent as a bearer token.\n  sources:\n  - openapi/tesseralytics-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tesseralytics-dev/authentication/tesseralytics-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- MarketData
- Analytics
- API
---
