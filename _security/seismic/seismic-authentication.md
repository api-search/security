---
api_key_in: []
api_specs:
- filename: seismic-content-analytics-api-openapi.yml
  format: yaml
  label: Seismic Content Analytics API
  slug: seismic-content-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-analytics-api-openapi.yml
- filename: seismic-content-api-openapi.yml
  format: yaml
  label: Seismic Content API
  slug: seismic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-api-openapi.yml
- filename: seismic-content-profiles-api-openapi.yml
  format: yaml
  label: Seismic Content Profiles API
  slug: seismic-content-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-profiles-api-openapi.yml
- filename: seismic-content-properties-api-openapi.yml
  format: yaml
  label: Seismic Content Properties API
  slug: seismic-content-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-properties-api-openapi.yml
- filename: seismic-data-sources-api-openapi.yml
  format: yaml
  label: Seismic Data Sources API
  slug: seismic-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-data-sources-api-openapi.yml
- filename: seismic-delivery-analytics-api-openapi.yml
  format: yaml
  label: Seismic Delivery Analytics API
  slug: seismic-delivery-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-analytics-api-openapi.yml
- filename: seismic-delivery-api-openapi.yml
  format: yaml
  label: Seismic Delivery API
  slug: seismic-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-api-openapi.yml
- filename: seismic-folders-api-openapi.yml
  format: yaml
  label: Seismic Folders API
  slug: seismic-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-folders-api-openapi.yml
- filename: seismic-generation-jobs-api-openapi.yml
  format: yaml
  label: Seismic Generation Jobs API
  slug: seismic-generation-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-generation-jobs-api-openapi.yml
- filename: seismic-groups-api-openapi.yml
  format: yaml
  label: Seismic Groups API
  slug: seismic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-groups-api-openapi.yml
- filename: seismic-livedocs-api-openapi.yml
  format: yaml
  label: Seismic LiveDocs API
  slug: seismic-livedocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-livedocs-api-openapi.yml
- filename: seismic-reports-api-openapi.yml
  format: yaml
  label: Seismic Reports API
  slug: seismic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-reports-api-openapi.yml
- filename: seismic-roles-api-openapi.yml
  format: yaml
  label: Seismic Roles API
  slug: seismic-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-roles-api-openapi.yml
- filename: seismic-teams-api-openapi.yml
  format: yaml
  label: Seismic Teams API
  slug: seismic-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-teams-api-openapi.yml
- filename: seismic-templates-api-openapi.yml
  format: yaml
  label: Seismic Templates API
  slug: seismic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-templates-api-openapi.yml
- filename: seismic-user-analytics-api-openapi.yml
  format: yaml
  label: Seismic User Analytics API
  slug: seismic-user-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-user-analytics-api-openapi.yml
- filename: seismic-users-api-openapi.yml
  format: yaml
  label: Seismic Users API
  slug: seismic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Seismic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seismic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seismic
provider_slug: seismic
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer Token. Obtain tokens through the Seismic authentication flow. See https://developer.seismic.com/seismicsoftware/docs/authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/seismic-analytics-openapi.yml
  - openapi/seismic-content-openapi.yml
  - openapi/seismic-livedocs-openapi.yml
  - openapi/seismic-user-management-openapi.yml
  type: http
slug: seismic-authentication
source_filename: seismic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seismic-analytics-openapi.yml, openapi/seismic-content-openapi.yml, openapi/seismic-livedocs-openapi.yml,\n  openapi/seismic-user-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer Token. Obtain tokens through the Seismic authentication flow.\n    See https://developer.seismic.com/seismicsoftware/docs/authentication\n  sources:\n  - openapi/seismic-analytics-openapi.yml\n  - openapi/seismic-content-openapi.yml\n  - openapi/seismic-livedocs-openapi.yml\n  - openapi/seismic-user-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/authentication/seismic-authentication.yml
summary_line: http · 1 scheme
tags: []
---
