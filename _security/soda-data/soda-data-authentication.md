---
api_key_in: []
api_specs:
- filename: soda-data-attributes-api-openapi.yml
  format: yaml
  label: Soda Attributes API
  slug: soda-data-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-attributes-api-openapi.yml
- filename: soda-data-authentication-api-openapi.yml
  format: yaml
  label: Soda Authentication API
  slug: soda-data-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-authentication-api-openapi.yml
- filename: soda-data-checks-api-openapi.yml
  format: yaml
  label: Soda Checks API
  slug: soda-data-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-checks-api-openapi.yml
- filename: soda-data-contracts-api-openapi.yml
  format: yaml
  label: Soda Contracts API
  slug: soda-data-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-contracts-api-openapi.yml
- filename: soda-data-datasets-api-openapi.yml
  format: yaml
  label: Soda Datasets API
  slug: soda-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-datasets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soda Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soda
provider_slug: soda-data
scheme_count: 1
schemes:
- description: Basic HTTP authentication using Base64-encoded `api_key_id:api_key_secret`.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/soda-data-openapi.yml
  type: http
slug: soda-data-authentication
source_filename: soda-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soda-data-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic HTTP authentication using Base64-encoded `api_key_id:api_key_secret`.\n  sources:\n  - openapi/soda-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/authentication/soda-data-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Data Quality
---
