---
api_key_in: []
api_specs:
- filename: antimetal-artifacts-api-openapi.yml
  format: yaml
  label: Antimetal Artifacts API
  slug: antimetal-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-artifacts-api-openapi.yml
- filename: antimetal-issues-api-openapi.yml
  format: yaml
  label: Antimetal Issues API
  slug: antimetal-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-issues-api-openapi.yml
- filename: antimetal-query-api-openapi.yml
  format: yaml
  label: Antimetal Query API
  slug: antimetal-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-query-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Antimetal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Antimetal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Antimetal
provider_slug: antimetal
scheme_count: 1
schemes:
- description: API key authentication via Bearer token
  name: bearer
  scheme: bearer
  sources:
  - openapi/antimetal-external-api-openapi.json
  type: http
slug: antimetal-authentication
source_filename: antimetal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/antimetal-external-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key authentication via Bearer token\n  sources:\n  - openapi/antimetal-external-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/authentication/antimetal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Observability
- Incident Management
- Site Reliability Engineering
- Artificial Intelligence
- Agents
- DevOps
- Cloud Infrastructure
- Kubernetes
- Root Cause Analysis
- MCP
---
