---
api_key_in: []
api_specs:
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Workspaces API
  slug: gooddata-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Data Sources API
  slug: gooddata-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Logical Data Model API
  slug: gooddata-logical-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Metrics API
  slug: gooddata-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Visualizations & Dashboards API
  slug: gooddata-visualizations-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Execution / AFM API
  slug: gooddata-execution-afm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Users & Permissions API
  slug: gooddata-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gooddata Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoodData secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoodData
provider_slug: gooddata
scheme_count: 1
schemes:
- description: 'GoodData Cloud API token passed as ''Authorization: Bearer <API_TOKEN>''.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gooddata-openapi.yml
  type: http
slug: gooddata-authentication
source_filename: gooddata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gooddata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'GoodData Cloud API token passed as ''Authorization: Bearer <API_TOKEN>''.'\n  sources:\n  - openapi/gooddata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/authentication/gooddata-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Dashboards
- Data
---
