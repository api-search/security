---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: netapi-com-free-datasets-api-openapi.yml
  format: yaml
  label: NetAPI Telecom Free Datasets API
  slug: netapi-com-free-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-free-datasets-api-openapi.yml
- filename: netapi-com-json-api-api-openapi.yml
  format: yaml
  label: NetAPI Telecom JSON API
  slug: netapi-com-json-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-json-api-api-openapi.yml
- filename: netapi-com-reference-api-openapi.yml
  format: yaml
  label: NetAPI Telecom Reference API
  slug: netapi-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-reference-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NetAPI Telecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetAPI Telecom secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetAPI Telecom
provider_slug: netapi-com
scheme_count: 2
schemes:
- description: API token from https://netapi.com/dashboard/
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/netapi-com-openapi.yml
  type: apiKey
- description: The same API token in the Authorization header (JSON API); OAuth access tokens issued by https://netapi.com are accepted too.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/netapi-com-openapi.yml
  type: http
slug: netapi-com-authentication
source_filename: netapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/netapi-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token from https://netapi.com/dashboard/\n  sources:\n  - openapi/netapi-com-openapi.yml\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: The same API token in the Authorization header (JSON API); OAuth access tokens\n    issued by https://netapi.com are accepted too.\n  sources:\n  - openapi/netapi-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/netapi-com/authentication/netapi-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Domain Lists
- DNS Data
- WHOIS
- Threat Intelligence
- Data Feed
---
