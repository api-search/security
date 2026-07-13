---
api_key_in: []
api_specs:
- filename: restack-openapi.yml
  format: yaml
  label: Restack
  slug: restack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/openapi/restack-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Restack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Restack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Restack
provider_slug: restack
scheme_count: 1
schemes:
- description: Bearer token for API authentication. Set via RESTACK_API_BEARER_TOKEN environment variable.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/restack-openapi.yml
  type: http
slug: restack-authentication
source_filename: restack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for API authentication. Set via RESTACK_API_BEARER_TOKEN environment\n    variable.\n  sources:\n  - openapi/restack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/authentication/restack-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Workflows
- Orchestration
- Enterprise
- Python
---
