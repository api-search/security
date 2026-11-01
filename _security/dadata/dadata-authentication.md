---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dadata-clean-openapi-generated.yml
  format: yaml
  label: DaData API-методы API
  slug: clean-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dadata/openapi/_ae-authored/dadata-clean-openapi-generated.yml
- filename: dadata-core-openapi-generated.yml
  format: yaml
  label: DaData core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dadata/openapi/_ae-authored/dadata-core-openapi-generated.yml
- filename: dadata-suggest-openapi-generated.yml
  format: yaml
  label: DaData API-методы API
  slug: suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dadata/openapi/_ae-authored/dadata-suggest-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dadata Authentication
name_suffix: Authentication
oauth_flows: []
overview: DaData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DaData
provider_slug: dadata
scheme_count: 1
schemes:
- description: 'API key provided by DaData, sent as ''Authorization: Token <API_KEY>'''
  in: header
  name: Authorization
  type: apiKey
slug: dadata-authentication
source_filename: dadata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://dadata.ru/docs/\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"API key provided by DaData, sent as 'Authorization: Token <API_KEY>'\"\n"
source_yaml_url: https://artifacts.apis.io/dadata/authentication/dadata-authentication.yml
summary_line: 1 scheme
tags:
- Data
- API
- Russian
- DataEnrichment
- AddressStandardization
---
