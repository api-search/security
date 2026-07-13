---
api_key_in: []
api_specs:
- filename: census-openapi.yml
  format: yaml
  label: Census Activations REST API
  slug: census-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Census Authentication
name_suffix: Authentication
oauth_flows: []
overview: Census secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Census
provider_slug: census
scheme_count: 1
schemes:
- description: Workspace access token or organization personal access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/census-openapi.yml
  type: http
slug: census-authentication
source_filename: census-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/census-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Workspace access token or organization personal access token\n  sources:\n  - openapi/census-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/authentication/census-authentication.yml
summary_line: http · 1 scheme
tags:
- Connectors
- Data Activation
- Data Warehouse
- Destinations
- Fivetran Activations
- Reverse ETL
- Unified API
---
