---
api_key_in: []
api_specs:
- filename: cortex-openapi.yml
  format: yaml
  label: Cortex REST API
  slug: cortex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex/refs/heads/main/openapi/cortex-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cortex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cortex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cortex
provider_slug: cortex
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cortex-openapi.yml
  type: http
slug: cortex-authentication
source_filename: cortex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cortex-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cortex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex/refs/heads/main/authentication/cortex-authentication.yml
summary_line: http · 1 scheme
tags:
- Catalog
- Custom Data
- Dependencies
- Deploys
- Developer Experience
- EngOps
- Engineering Intelligence
- Initiatives
- Internal Developer Portal
- On-call
- Platform Engineering
- Scorecards
- Service Catalog
- SRE
- Workflows
---
