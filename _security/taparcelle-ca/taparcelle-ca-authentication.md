---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: taparcelle-ca-decisions-api-openapi.yml
  format: yaml
  label: TaParcelle Decisions API
  slug: taparcelle-ca-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-decisions-api-openapi.yml
- filename: taparcelle-ca-demographics-api-openapi.yml
  format: yaml
  label: TaParcelle Demographics API
  slug: taparcelle-ca-demographics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-demographics-api-openapi.yml
- filename: taparcelle-ca-documents-api-openapi.yml
  format: yaml
  label: TaParcelle Documents API
  slug: taparcelle-ca-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-documents-api-openapi.yml
- filename: taparcelle-ca-parcels-api-openapi.yml
  format: yaml
  label: TaParcelle Parcels API
  slug: taparcelle-ca-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-parcels-api-openapi.yml
- filename: taparcelle-ca-search-api-openapi.yml
  format: yaml
  label: TaParcelle Search API
  slug: taparcelle-ca-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-search-api-openapi.yml
- filename: taparcelle-ca-sectors-api-openapi.yml
  format: yaml
  label: TaParcelle Sectors API
  slug: taparcelle-ca-sectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-sectors-api-openapi.yml
- filename: taparcelle-ca-usage-api-openapi.yml
  format: yaml
  label: TaParcelle Usage API
  slug: taparcelle-ca-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-usage-api-openapi.yml
- filename: taparcelle-ca-zoning-api-openapi.yml
  format: yaml
  label: TaParcelle Zoning API
  slug: taparcelle-ca-zoning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-zoning-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: TaParcelle Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaParcelle secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TaParcelle
provider_slug: taparcelle-ca
scheme_count: 2
schemes:
- in: header
  name: cleApi
  parameter: X-API-Key
  sources:
  - openapi/taparcelle-ca-openapi.json
  type: apiKey
- description: La même clé, en jeton porteur.
  name: jeton
  scheme: bearer
  sources:
  - openapi/taparcelle-ca-openapi.json
  type: http
slug: taparcelle-ca-authentication
source_filename: taparcelle-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/taparcelle-ca-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: cleApi\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/taparcelle-ca-openapi.json\n- name: jeton\n  type: http\n  scheme: bearer\n  description: La même clé, en jeton porteur.\n  sources:\n  - openapi/taparcelle-ca-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/taparcelle-ca/authentication/taparcelle-ca-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- RealEstate
- DataAggregation
- Quebec
- Property
- API
---
