---
api_key_in:
- header
api_specs:
- filename: cloudrf-3d-api-openapi.yml
  format: yaml
  label: CloudRF 3D API
  slug: cloudrf-3d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-3d-api-openapi.yml
- filename: cloudrf-account-api-openapi.yml
  format: yaml
  label: CloudRF Account API
  slug: cloudrf-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-account-api-openapi.yml
- filename: cloudrf-analyse-api-openapi.yml
  format: yaml
  label: CloudRF Analyse API
  slug: cloudrf-analyse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-analyse-api-openapi.yml
- filename: cloudrf-create-api-openapi.yml
  format: yaml
  label: CloudRF Create API
  slug: cloudrf-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-create-api-openapi.yml
- filename: cloudrf-manage-api-openapi.yml
  format: yaml
  label: CloudRF Manage API
  slug: cloudrf-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-manage-api-openapi.yml
- filename: cloudrf-satellite-api-openapi.yml
  format: yaml
  label: CloudRF Satellite API
  slug: cloudrf-satellite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-satellite-api-openapi.yml
- filename: cloudrf-template-api-openapi.yml
  format: yaml
  label: CloudRF Template API
  slug: cloudrf-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-template-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudrf Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudRF secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudRF
provider_slug: cloudrf
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/cloudrf-openapi.yml
  type: apiKey
slug: cloudrf-authentication
source_filename: cloudrf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudrf-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: key\n  sources:\n  - openapi/cloudrf-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/authentication/cloudrf-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Coverage Modeling
- HF Propagation
- Mesh Network
- Radio Frequency
- RF
- Satellite
- Signal Analysis
- Telecommunications
- Wireless Planning
---
