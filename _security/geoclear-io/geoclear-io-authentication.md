---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: geoclear-io-account-api-openapi.yml
  format: yaml
  label: GeoClear Account API
  slug: geoclear-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geoclear-io/openapi/geoclear-io-account-api-openapi.yml
- filename: geoclear-io-address-api-openapi.yml
  format: yaml
  label: GeoClear Address API
  slug: geoclear-io-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geoclear-io/openapi/geoclear-io-address-api-openapi.yml
- filename: geoclear-io-enrichment-api-openapi.yml
  format: yaml
  label: GeoClear Enrichment API
  slug: geoclear-io-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geoclear-io/openapi/geoclear-io-enrichment-api-openapi.yml
- filename: geoclear-io-geography-api-openapi.yml
  format: yaml
  label: GeoClear Geography API
  slug: geoclear-io-geography-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geoclear-io/openapi/geoclear-io-geography-api-openapi.yml
- filename: geoclear-io-status-api-openapi.yml
  format: yaml
  label: GeoClear Status API
  slug: geoclear-io-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geoclear-io/openapi/geoclear-io-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: GeoClear Authentication
name_suffix: Authentication
oauth_flows: []
overview: GeoClear secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GeoClear
provider_slug: geoclear-io
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/geoclear-io-dev-openapi.yaml
  - openapi/geoclear-io-openapi.yaml
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/geoclear-io-dev-openapi.yaml
  - openapi/geoclear-io-openapi.yaml
  type: apiKey
slug: geoclear-io-authentication
source_filename: geoclear-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/geoclear-io-dev-openapi.yaml, openapi/geoclear-io-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/geoclear-io-dev-openapi.yaml\n  - openapi/geoclear-io-openapi.yaml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/geoclear-io-dev-openapi.yaml\n  - openapi/geoclear-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/geoclear-io/authentication/geoclear-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Security
- Governance
- Cloud
- Enterprise
- Company
---
