---
api_key_in: []
api_specs:
- filename: teable-openapi.yml
  format: yaml
  label: Teable Spaces API
  slug: teable-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Bases API
  slug: teable-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Tables API
  slug: teable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Fields API
  slug: teable-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Records API
  slug: teable-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Views API
  slug: teable-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Attachments API
  slug: teable-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
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
