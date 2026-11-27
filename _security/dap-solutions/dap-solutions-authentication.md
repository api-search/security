---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dap-solutions-change-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Change API
  slug: dap-solutions-change-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-change-api-openapi.yml
- filename: dap-solutions-compute-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Compute API
  slug: dap-solutions-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-compute-api-openapi.yml
- filename: dap-solutions-compute-day-count-to-settlement-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Compute Day Count To Settlement API
  slug: dap-solutions-compute-day-count-to-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-compute-day-count-to-settlement-api-openapi.yml
- filename: dap-solutions-convert-unix-timestamp-to-date-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Convert Unix Timestamp To Date API
  slug: dap-solutions-convert-unix-timestamp-to-date-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-convert-unix-timestamp-to-date-api-openapi.yml
- filename: dap-solutions-coverage-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Coverage API
  slug: dap-solutions-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-coverage-api-openapi.yml
- filename: dap-solutions-decode-base64-to-text-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Decode Base64 To Text API
  slug: dap-solutions-decode-base64-to-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-decode-base64-to-text-api-openapi.yml
- filename: dap-solutions-diff-two-line-lists-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Diff Two Line Lists API
  slug: dap-solutions-diff-two-line-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-diff-two-line-lists-api-openapi.yml
- filename: dap-solutions-recent-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Recent API
  slug: dap-solutions-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-recent-api-openapi.yml
- filename: dap-solutions-search-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Search API
  slug: dap-solutions-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dartmouth Advisory Partners Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dartmouth Advisory Partners secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dartmouth Advisory Partners
provider_slug: dap-solutions
scheme_count: 2
schemes:
- description: A DAP licence key (dapk_...), issued to an institution under a licence and invoiced by usage. Contact bsibeth@dap.solutions.
  name: licenceKey
  scheme: bearer
  sources:
  - openapi/bellwether-openapi.json
  - openapi/compute-openapi.json
  type: http
- description: The same DAP licence key, for platforms that set an API key header.
  in: header
  name: licenceKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/bellwether-openapi.json
  - openapi/compute-openapi.json
  type: apiKey
slug: dap-solutions-authentication
source_filename: dap-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/bellwether-openapi.json, openapi/compute-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: licenceKey\n  type: http\n  scheme: bearer\n  description: A DAP licence key (dapk_...), issued to an institution under a licence and invoiced\n    by usage. Contact bsibeth@dap.solutions.\n  sources:\n  - openapi/bellwether-openapi.json\n  - openapi/compute-openapi.json\n- name: licenceKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The same DAP licence key, for platforms that set an API key header.\n  sources:\n  - openapi/bellwether-openapi.json\n  - openapi/compute-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dap-solutions/authentication/dap-solutions-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Governance
- Artificial Intelligence
- Toronto
- Institutional
- Technology
- Company
---
