---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cenogram-pl-demographics-api-openapi.yml
  format: yaml
  label: Cenogram Demographics API
  slug: cenogram-pl-demographics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-demographics-api-openapi.yml
- filename: cenogram-pl-infrastructure-api-openapi.yml
  format: yaml
  label: Cenogram Infrastructure API
  slug: cenogram-pl-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-infrastructure-api-openapi.yml
- filename: cenogram-pl-locations-api-openapi.yml
  format: yaml
  label: Cenogram Locations API
  slug: cenogram-pl-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-locations-api-openapi.yml
- filename: cenogram-pl-parcels-api-openapi.yml
  format: yaml
  label: Cenogram Parcels API
  slug: cenogram-pl-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-parcels-api-openapi.yml
- filename: cenogram-pl-spatial-api-openapi.yml
  format: yaml
  label: Cenogram Spatial API
  slug: cenogram-pl-spatial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-spatial-api-openapi.yml
- filename: cenogram-pl-statistics-api-openapi.yml
  format: yaml
  label: Cenogram Statistics API
  slug: cenogram-pl-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-statistics-api-openapi.yml
- filename: cenogram-pl-transactions-api-openapi.yml
  format: yaml
  label: Cenogram Transactions API
  slug: cenogram-pl-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-transactions-api-openapi.yml
- filename: cenogram-pl-districts-api-openapi.yml
  format: yaml
  label: Cenogram Districts API
  slug: cenogram-pl-districts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-districts-api-openapi.yml
- filename: cenogram-pl-infrastructure-signals-api-openapi.yml
  format: yaml
  label: Cenogram Infrastructure Signals API
  slug: cenogram-pl-infrastructure-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-infrastructure-signals-api-openapi.yml
- filename: cenogram-pl-permits-api-openapi.yml
  format: yaml
  label: Cenogram Permits API
  slug: cenogram-pl-permits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-permits-api-openapi.yml
- filename: cenogram-pl-price-per-m2-api-openapi.yml
  format: yaml
  label: Cenogram Price Per M2 API
  slug: cenogram-pl-price-per-m2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-price-per-m2-api-openapi.yml
- filename: cenogram-pl-stats-api-openapi.yml
  format: yaml
  label: Cenogram Stats API
  slug: cenogram-pl-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-stats-api-openapi.yml
- filename: cenogram-pl-streets-api-openapi.yml
  format: yaml
  label: Cenogram Streets API
  slug: cenogram-pl-streets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-streets-api-openapi.yml
- filename: cenogram-pl-valuations-api-openapi.yml
  format: yaml
  label: Cenogram Valuations API
  slug: cenogram-pl-valuations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-valuations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cenogram Pl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cenogram secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cenogram
provider_slug: cenogram-pl
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/cenogram-pl-openapi.json
  type: apiKey
slug: cenogram-pl-authentication
source_filename: cenogram-pl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cenogram-pl-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/cenogram-pl-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cenogram-pl/authentication/cenogram-pl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Real Estate
- Data
- Analytics
- Poland
---
