---
api_key_in:
- header
api_specs:
- filename: people-data-labs-autocomplete-api-openapi.yml
  format: yaml
  label: People Data Labs Autocomplete API
  slug: people-data-labs-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-autocomplete-api-openapi.yml
- filename: people-data-labs-company-api-openapi.yml
  format: yaml
  label: People Data Labs Company API
  slug: people-data-labs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-company-api-openapi.yml
- filename: people-data-labs-ip-api-openapi.yml
  format: yaml
  label: People Data Labs IP API
  slug: people-data-labs-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-ip-api-openapi.yml
- filename: people-data-labs-jobs-api-openapi.yml
  format: yaml
  label: People Data Labs Jobs API
  slug: people-data-labs-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-jobs-api-openapi.yml
- filename: people-data-labs-person-api-openapi.yml
  format: yaml
  label: People Data Labs Person API
  slug: people-data-labs-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-person-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: People Data Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: People Data Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: People Data Labs
provider_slug: people-data-labs
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/people-data-labs-openapi.yml
  type: apiKey
slug: people-data-labs-authentication
source_filename: people-data-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/people-data-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/people-data-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/authentication/people-data-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Identity Resolution
- People Data
---
