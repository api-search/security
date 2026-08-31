---
api_key_in:
- header
api_specs:
- filename: optilogic-authentication-api-openapi.yml
  format: yaml
  label: Optilogic Authentication API
  slug: optilogic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-authentication-api-openapi.yml
- filename: optilogic-job-api-openapi.yml
  format: yaml
  label: Optilogic Job API
  slug: optilogic-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-job-api-openapi.yml
- filename: optilogic-storage-api-openapi.yml
  format: yaml
  label: Optilogic Storage API
  slug: optilogic-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-api-openapi.yml
- filename: optilogic-storage-custom-columns-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : custom columns API'
  slug: optilogic-storage-custom-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-custom-columns-api-openapi.yml
- filename: optilogic-storage-custom-tables-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : custom tables API'
  slug: optilogic-storage-custom-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-custom-tables-api-openapi.yml
- filename: optilogic-storage-labels-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : labels API'
  slug: optilogic-storage-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-labels-api-openapi.yml
- filename: optilogic-storage-sharing-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : sharing API'
  slug: optilogic-storage-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-sharing-api-openapi.yml
- filename: optilogic-storage-tags-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : tags API'
  slug: optilogic-storage-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-tags-api-openapi.yml
- filename: optilogic-storage-templates-api-openapi.yml
  format: yaml
  label: 'Optilogic storage : templates API'
  slug: optilogic-storage-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-storage-templates-api-openapi.yml
- filename: optilogic-utility-api-openapi.yml
  format: yaml
  label: Optilogic Utility API
  slug: optilogic-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-utility-api-openapi.yml
- filename: optilogic-workspace-api-openapi.yml
  format: yaml
  label: Optilogic Workspace API
  slug: optilogic-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Optilogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optilogic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Optilogic
provider_slug: optilogic
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/optilogic-rest-api-openapi.json
  type: apiKey
slug: optilogic-authentication
source_filename: optilogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/optilogic-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/optilogic-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/authentication/optilogic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Supply Chain Design
- Network Optimization
- Simulation
- Optimization
- Logistics
- Analytics
- Artificial Intelligence
- Job
- Cloud
---
