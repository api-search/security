---
api_key_in:
- header
api_specs:
- filename: keen-event-collection-api-openapi.yml
  format: yaml
  label: Keen Event Collection API
  slug: event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-event-collection-api-openapi.yml
- filename: keen-query-api-openapi.yml
  format: yaml
  label: Keen Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-query-api-openapi.yml
- filename: keen-cached-queries-api-openapi.yml
  format: yaml
  label: Keen Cached Queries API
  slug: cached-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-cached-queries-api-openapi.yml
- filename: keen-saved-queries-api-openapi.yml
  format: yaml
  label: Keen Saved Queries API
  slug: saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-saved-queries-api-openapi.yml
- filename: keen-data-extraction-api-openapi.yml
  format: yaml
  label: Keen Data Extraction API
  slug: data-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-data-extraction-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Keen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keen secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keen
provider_slug: keen
scheme_count: 1
schemes:
- description: Keen Master Key for management endpoints.
  in: header
  name: masterKey
  parameter: Authorization
  sources:
  - openapi/keen-cached-queries-api-openapi.yml
  - openapi/keen-data-extraction-api-openapi.yml
  - openapi/keen-event-collection-api-openapi.yml
  - openapi/keen-query-api-openapi.yml
  - openapi/keen-saved-queries-api-openapi.yml
  type: apiKey
slug: keen-authentication
source_filename: keen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keen-cached-queries-api-openapi.yml, openapi/keen-data-extraction-api-openapi.yml,\n  openapi/keen-event-collection-api-openapi.yml, openapi/keen-query-api-openapi.yml, openapi/keen-saved-queries-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: masterKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Keen Master Key for management endpoints.\n  sources:\n  - openapi/keen-cached-queries-api-openapi.yml\n  - openapi/keen-data-extraction-api-openapi.yml\n  - openapi/keen-event-collection-api-openapi.yml\n  - openapi/keen-query-api-openapi.yml\n  - openapi/keen-saved-queries-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/authentication/keen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Custom Events
- Data Collection
- Embedded Analytics
- Event Analytics
---
