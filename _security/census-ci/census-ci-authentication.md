---
api_key_in: []
api_specs:
- filename: census-ci-connectors-api-openapi.yml
  format: yaml
  label: Census Connectors API
  slug: census-ci-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-connectors-api-openapi.yml
- filename: census-ci-datasets-and-models-api-openapi.yml
  format: yaml
  label: Census Datasets and Models API
  slug: census-ci-datasets-and-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-datasets-and-models-api-openapi.yml
- filename: census-ci-destinations-api-openapi.yml
  format: yaml
  label: Census Destinations API
  slug: census-ci-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-destinations-api-openapi.yml
- filename: census-ci-segments-api-openapi.yml
  format: yaml
  label: Census Segments API
  slug: census-ci-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-segments-api-openapi.yml
- filename: census-ci-sources-api-openapi.yml
  format: yaml
  label: Census Sources API
  slug: census-ci-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-sources-api-openapi.yml
- filename: census-ci-sync-runs-api-openapi.yml
  format: yaml
  label: Census Sync Runs API
  slug: census-ci-sync-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-sync-runs-api-openapi.yml
- filename: census-ci-syncs-api-openapi.yml
  format: yaml
  label: Census Syncs API
  slug: census-ci-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/openapi/census-ci-syncs-api-openapi.yml
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
