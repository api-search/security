---
api_key_in:
- header
api_specs:
- filename: pixxel-aoi-api-openapi.yml
  format: yaml
  label: Pixxel AOI API
  slug: pixxel-aoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-aoi-api-openapi.yml
- filename: pixxel-archives-api-openapi.yml
  format: yaml
  label: Pixxel Archives API
  slug: pixxel-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-archives-api-openapi.yml
- filename: pixxel-assets-api-openapi.yml
  format: yaml
  label: Pixxel Assets API
  slug: pixxel-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-assets-api-openapi.yml
- filename: pixxel-bandset-api-openapi.yml
  format: yaml
  label: Pixxel Bandset API
  slug: pixxel-bandset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-bandset-api-openapi.yml
- filename: pixxel-blocks-api-openapi.yml
  format: yaml
  label: Pixxel Blocks API
  slug: pixxel-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-blocks-api-openapi.yml
- filename: pixxel-catalog-api-openapi.yml
  format: yaml
  label: Pixxel Catalog API
  slug: pixxel-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-catalog-api-openapi.yml
- filename: pixxel-downloads-api-openapi.yml
  format: yaml
  label: Pixxel Downloads API
  slug: pixxel-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-downloads-api-openapi.yml
- filename: pixxel-external-api-openapi.yml
  format: yaml
  label: Pixxel external API
  slug: pixxel-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-external-api-openapi.yml
- filename: pixxel-indices-api-openapi.yml
  format: yaml
  label: Pixxel Indices API
  slug: pixxel-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-indices-api-openapi.yml
- filename: pixxel-insights-api-openapi.yml
  format: yaml
  label: Pixxel Insights API
  slug: pixxel-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-insights-api-openapi.yml
- filename: pixxel-jobs-api-openapi.yml
  format: yaml
  label: Pixxel Jobs API
  slug: pixxel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-jobs-api-openapi.yml
- filename: pixxel-order-api-openapi.yml
  format: yaml
  label: Pixxel Order API
  slug: pixxel-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-order-api-openapi.yml
- filename: pixxel-project-api-openapi.yml
  format: yaml
  label: Pixxel Project API
  slug: pixxel-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-project-api-openapi.yml
- filename: pixxel-report-api-openapi.yml
  format: yaml
  label: Pixxel Report API
  slug: pixxel-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-report-api-openapi.yml
- filename: pixxel-search-api-openapi.yml
  format: yaml
  label: Pixxel Search API
  slug: pixxel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-search-api-openapi.yml
- filename: pixxel-stores-api-openapi.yml
  format: yaml
  label: Pixxel Stores API
  slug: pixxel-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-stores-api-openapi.yml
- filename: pixxel-tasks-api-openapi.yml
  format: yaml
  label: Pixxel Tasks API
  slug: pixxel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-tasks-api-openapi.yml
- filename: pixxel-visualizations-api-openapi.yml
  format: yaml
  label: Pixxel Visualizations API
  slug: pixxel-visualizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-visualizations-api-openapi.yml
- filename: pixxel-workflows-api-openapi.yml
  format: yaml
  label: Pixxel Workflows API
  slug: pixxel-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pixxel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixxel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixxel
provider_slug: pixxel
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  scheme_detail: Bearer Personal Access Token
  sources:
  - openapi/pixxel-openapi-original.json
  type: apiKey
slug: pixxel-authentication
source_filename: pixxel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pixxel-openapi-original.json\ndocs: https://docs.pixxel.space/developer/gettingstarted/authentication.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: Personal Access Token (bearer)\n  header: 'Authorization: Bearer <PERSONAL_ACCESS_TOKEN>'\n  scoped_by:\n  - organization\n  - project\n  - role\n  provisioning: Aurora platform -> Settings -> Personal Access Tokens (name, roles, project access, expiry).\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_detail: Bearer Personal Access Token\n  sources:\n  - openapi/pixxel-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/authentication/pixxel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Satellite Imagery
- Earth Observation
- Hyperspectral
- Geospatial
- Remote Sensing
- Analytics
- STAC
---
