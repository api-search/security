---
api_key_in:
- header
api_specs:
- filename: wundergraph-cosmo-platform-openapi.yml
  format: yaml
  label: WunderGraph Cosmo Platform API
  slug: cosmo-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-cosmo-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wundergraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: WunderGraph secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WunderGraph
provider_slug: wundergraph
scheme_count: 1
schemes:
- description: API key for authenticating with the Cosmo Platform API. Obtain via Cosmo Studio or wgc CLI. Set as COSMO_API_KEY environment variable.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/wundergraph-cosmo-platform-openapi.yml
  type: apiKey
slug: wundergraph-authentication
source_filename: wundergraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wundergraph-cosmo-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authenticating with the Cosmo Platform API. Obtain via Cosmo Studio\n    or wgc CLI. Set as COSMO_API_KEY environment variable.\n  sources:\n  - openapi/wundergraph-cosmo-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/authentication/wundergraph-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federation
- GraphQL
- Management
- Schema Registry
---
