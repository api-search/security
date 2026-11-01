---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dsrv-ethereum-api-openapi.yml
  format: yaml
  label: Dsrv Ethereum API
  slug: dsrv-ethereum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-ethereum-api-openapi.yml
- filename: dsrv-health-api-openapi.yml
  format: yaml
  label: Dsrv Health API
  slug: dsrv-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-health-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dsrv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dsrv secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dsrv
provider_slug: dsrv
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/dsrv-staking-hub-api-openapi.yml
  type: apiKey
slug: dsrv-authentication
source_filename: dsrv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: derived\nsource: openapi/dsrv-staking-hub-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication\n  sources:\n  - openapi/dsrv-staking-hub-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dsrv/authentication/dsrv-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Infrastructure
- Staking
- Web3
---
