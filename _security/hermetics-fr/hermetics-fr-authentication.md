---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hermetics-fr-law-api-openapi.yml
  format: yaml
  label: Hermetics Law API
  slug: hermetics-fr-law-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-law-api-openapi.yml
- filename: hermetics-fr-mcp-api-openapi.yml
  format: yaml
  label: Hermetics MCP API
  slug: hermetics-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-mcp-api-openapi.yml
- filename: hermetics-fr-records-api-openapi.yml
  format: yaml
  label: Hermetics Records API
  slug: hermetics-fr-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-records-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hermetics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hermetics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hermetics
provider_slug: hermetics-fr
scheme_count: 1
schemes:
- description: A Hermetics key (hk_...), created at https://hermetics.fr/mcp/cle with a free account.
  name: bearer
  scheme: bearer
  sources:
  - openapi/hermetics-fr-openapi.json
  type: http
slug: hermetics-fr-authentication
source_filename: hermetics-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hermetics-fr-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A Hermetics key (hk_...), created at https://hermetics.fr/mcp/cle with a free\n    account.\n  sources:\n  - openapi/hermetics-fr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hermetics-fr/authentication/hermetics-fr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
