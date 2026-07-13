---
api_key_in: []
api_specs:
- filename: core
  format: yaml
  label: Twenty Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://api.twenty.com/open-api/core
- filename: metadata
  format: yaml
  label: Twenty Metadata API
  slug: metadata-api
  spec_type: OpenAPI
  url: https://api.twenty.com/open-api/metadata
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Twenty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twenty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Twenty
provider_slug: twenty
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Workspace-scoped Bearer token. Generate from Settings → Playground in your Twenty workspace.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/twenty-core-api-openapi.yml
  - openapi/twenty-metadata-api-openapi.yml
  type: http
slug: twenty-authentication
source_filename: twenty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twenty-core-api-openapi.yml, openapi/twenty-metadata-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Workspace-scoped Bearer token. Generate from Settings → Playground in your Twenty\n    workspace.\n  sources:\n  - openapi/twenty-core-api-openapi.yml\n  - openapi/twenty-metadata-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/authentication/twenty-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Open Source
- REST
- GraphQL
- Webhooks
- Self-Hosted
- Companies
- People
- Opportunities
- Workflows
- AI Agents
- Custom Objects
---
