---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: zentriaflow-com-free-tools-api-openapi.yml
  format: yaml
  label: Zentria Flow Free tools API
  slug: zentriaflow-com-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zentriaflow-com/openapi/zentriaflow-com-free-tools-api-openapi.yml
- filename: zentriaflow-com-keyed-api-api-openapi.yml
  format: yaml
  label: Zentria Flow Keyed API
  slug: zentriaflow-com-keyed-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zentriaflow-com/openapi/zentriaflow-com-keyed-api-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Zentria Flow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zentria Flow secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zentria Flow
provider_slug: zentriaflow-com
scheme_count: 2
schemes:
- description: Your key, which starts with `zf_live_`.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/zentriaflow-com-openapi.json
  type: apiKey
- description: 'The same key as a bearer token: `Authorization: Bearer zf_live_...`.'
  name: BearerKey
  scheme: bearer
  sources:
  - openapi/zentriaflow-com-openapi.json
  type: http
slug: zentriaflow-com-authentication
source_filename: zentriaflow-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/zentriaflow-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your key, which starts with `zf_live_`.\n  sources:\n  - openapi/zentriaflow-com-openapi.json\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: 'The same key as a bearer token: `Authorization: Bearer zf_live_...`.'\n  sources:\n  - openapi/zentriaflow-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/zentriaflow-com/authentication/zentriaflow-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Import
- Tariffs
- Landed Cost
---
