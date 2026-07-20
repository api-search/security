---
api_key_in:
- header
api_specs:
- filename: edge-delta-openapi-original.json
  format: json
  label: Edge Delta API
  slug: edge-delta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Edge Delta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edge Delta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edge Delta
provider_slug: edge-delta
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-ED-API-Token
  sources:
  - openapi/edge-delta-openapi-original.json
  type: apiKey
slug: edge-delta-authentication
source_filename: edge-delta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/edge-delta-openapi-original.json\ndocs: https://docs.edgedelta.com/api-tokens/\nnotes: >-\n  Per-organization API token passed in the X-ED-API-Token header. Tokens are\n  created at https://docs.edgedelta.com/create-api-token/; the organization ID\n  (used in the {org_id} path scope) is obtained per https://docs.edgedelta.com/get-org-id/.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ED-API-Token\n  sources:\n  - openapi/edge-delta-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/authentication/edge-delta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Telemetry Pipelines
- Logging
- Metrics
- Tracing
- Monitoring
- DevOps
- SRE
- AI
---
