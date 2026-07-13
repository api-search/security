---
api_key_in: []
api_specs:
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Sources API
  slug: census-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Destinations API
  slug: census-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Syncs API
  slug: census-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Sync Runs API
  slug: census-sync-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Datasets & Models API
  slug: census-datasets-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Connections API
  slug: census-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
- filename: census-ci-openapi.yml
  format: yaml
  label: Census Segments & Audiences API
  slug: census-segments-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Census Ci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Census secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Census
provider_slug: census-ci
scheme_count: 1
schemes:
- description: Workspace API access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/census-ci-openapi.yml
  type: http
slug: census-ci-authentication
source_filename: census-ci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/census-ci-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Workspace API access token passed as a Bearer token.\n  sources:\n  - openapi/census-ci-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/authentication/census-ci-authentication.yml
summary_line: http · 1 scheme
tags:
- Reverse ETL
- Data Activation
- Data Warehouse
- Syncs
- Audience Hub
- Data Marketing
---
