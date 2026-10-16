---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: compabase-companies-api-openapi.yml
  format: yaml
  label: Compabase Companies API
  slug: compabase-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/openapi/compabase-companies-api-openapi.yml
- filename: compabase-health-api-openapi.yml
  format: yaml
  label: Compabase Health API
  slug: compabase-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/openapi/compabase-health-api-openapi.yml
- filename: compabase-persons-api-openapi.yml
  format: yaml
  label: Compabase Persons API
  slug: compabase-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/openapi/compabase-persons-api-openapi.yml
- filename: compabase-usage-api-openapi.yml
  format: yaml
  label: Compabase Usage API
  slug: compabase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/openapi/compabase-usage-api-openapi.yml
- filename: compabase-watchlist-api-openapi.yml
  format: yaml
  label: Compabase Watchlist API
  slug: compabase-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/openapi/compabase-watchlist-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Compabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compabase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Compabase
provider_slug: compabase
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/compabase-openapi.yaml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/compabase-openapi.yaml
  type: http
slug: compabase-authentication
source_filename: compabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/compabase-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/compabase-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/compabase-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compabase/refs/heads/main/authentication/compabase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Data
- Polish
- Business
- API
---
