---
api_key_in:
- header
api_specs:
- filename: softr-databases-api-openapi.yml
  format: yaml
  label: Softr Databases API
  slug: softr-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/openapi/softr-databases-api-openapi.yml
- filename: softr-records-api-openapi.yml
  format: yaml
  label: Softr Records API
  slug: softr-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/openapi/softr-records-api-openapi.yml
- filename: softr-users-api-openapi.yml
  format: yaml
  label: Softr Users API
  slug: softr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/openapi/softr-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Softr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Softr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Softr
provider_slug: softr
scheme_count: 1
schemes:
- description: Personal access token generated from the Softr workspace settings.
  in: header
  name: SoftrApiKey
  parameter: Softr-Api-Key
  sources:
  - openapi/softr-openapi.yml
  type: apiKey
slug: softr-authentication
source_filename: softr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/softr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SoftrApiKey\n  type: apiKey\n  in: header\n  parameter: Softr-Api-Key\n  description: Personal access token generated from the Softr workspace settings.\n  sources:\n  - openapi/softr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/authentication/softr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- No-Code
- App Builder
- Client Portals
- User Management
- Database
---
