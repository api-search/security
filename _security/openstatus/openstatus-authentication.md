---
api_key_in:
- header
api_specs:
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Monitors
  slug: monitors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Incidents
  slug: incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Reports
  slug: status-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Pages
  slug: status-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Checks
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openstatus Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenStatus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenStatus
provider_slug: openstatus
scheme_count: 1
schemes:
- description: OpenStatus API key, created in the workspace settings.
  in: header
  name: apiKey
  parameter: x-openstatus-key
  sources:
  - openapi/openstatus-openapi.yml
  type: apiKey
slug: openstatus-authentication
source_filename: openstatus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openstatus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-openstatus-key\n  description: OpenStatus API key, created in the workspace settings.\n  sources:\n  - openapi/openstatus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/authentication/openstatus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Monitoring
- Synthetic Monitoring
- Uptime
- Status Pages
- Incidents
- Open Source
- Observability
---
