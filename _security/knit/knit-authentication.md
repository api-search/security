---
api_key_in:
- header
api_specs:
- filename: knit-departments-api-openapi.yml
  format: yaml
  label: Knit Departments API
  slug: knit-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-departments-api-openapi.yml
- filename: knit-employees-api-openapi.yml
  format: yaml
  label: Knit Employees API
  slug: knit-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-employees-api-openapi.yml
- filename: knit-integrations-api-openapi.yml
  format: yaml
  label: Knit Integrations API
  slug: knit-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-integrations-api-openapi.yml
- filename: knit-jobs-api-openapi.yml
  format: yaml
  label: Knit Jobs API
  slug: knit-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-jobs-api-openapi.yml
- filename: knit-locations-api-openapi.yml
  format: yaml
  label: Knit Locations API
  slug: knit-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-locations-api-openapi.yml
- filename: knit-syncs-api-openapi.yml
  format: yaml
  label: Knit Syncs API
  slug: knit-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-syncs-api-openapi.yml
- filename: knit-time-off-api-openapi.yml
  format: yaml
  label: Knit Time Off API
  slug: knit-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-time-off-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Knit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knit
provider_slug: knit
scheme_count: 1
schemes:
- description: API key authentication via Bearer token.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/knit-unified-api-openapi.yml
  type: apiKey
slug: knit-authentication
source_filename: knit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knit-unified-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication via Bearer token.\n  sources:\n  - openapi/knit-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/authentication/knit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- HR Integrations
- HRIS
- Unified-API
---
