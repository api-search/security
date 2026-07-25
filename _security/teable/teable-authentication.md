---
api_key_in: []
api_specs:
- filename: teable-attachment-api-openapi.yml
  format: yaml
  label: Teable Attachment API
  slug: teable-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-attachment-api-openapi.yml
- filename: teable-base-api-openapi.yml
  format: yaml
  label: Teable Base API
  slug: teable-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-base-api-openapi.yml
- filename: teable-field-api-openapi.yml
  format: yaml
  label: Teable Field API
  slug: teable-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-field-api-openapi.yml
- filename: teable-record-api-openapi.yml
  format: yaml
  label: Teable Record API
  slug: teable-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-record-api-openapi.yml
- filename: teable-space-api-openapi.yml
  format: yaml
  label: Teable Space API
  slug: teable-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-space-api-openapi.yml
- filename: teable-table-api-openapi.yml
  format: yaml
  label: Teable Table API
  slug: teable-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-table-api-openapi.yml
- filename: teable-view-api-openapi.yml
  format: yaml
  label: Teable View API
  slug: teable-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-view-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teable
provider_slug: teable
scheme_count: 1
schemes:
- description: 'Personal access token or OAuth access token passed as `Authorization: Bearer {access_token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teable-openapi.yml
  type: http
slug: teable-authentication
source_filename: teable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token or OAuth access token passed as `Authorization: Bearer\n    {access_token}`.'\n  sources:\n  - openapi/teable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/authentication/teable-authentication.yml
summary_line: http · 1 scheme
tags:
- No-Code
- Database
- Airtable Alternative
- Postgres
- Open Source
---
