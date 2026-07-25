---
api_key_in: []
api_specs:
- filename: twenty-companies-api-openapi.yml
  format: yaml
  label: Twenty companies API
  slug: twenty-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-companies-api-openapi.yml
- filename: twenty-fields-api-openapi.yml
  format: yaml
  label: Twenty fields API
  slug: twenty-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-fields-api-openapi.yml
- filename: twenty-notes-api-openapi.yml
  format: yaml
  label: Twenty notes API
  slug: twenty-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-notes-api-openapi.yml
- filename: twenty-objects-api-openapi.yml
  format: yaml
  label: Twenty objects API
  slug: twenty-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-objects-api-openapi.yml
- filename: twenty-openapi-api-openapi.yml
  format: yaml
  label: Twenty openapi API
  slug: twenty-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-openapi-api-openapi.yml
- filename: twenty-opportunities-api-openapi.yml
  format: yaml
  label: Twenty opportunities API
  slug: twenty-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-opportunities-api-openapi.yml
- filename: twenty-people-api-openapi.yml
  format: yaml
  label: Twenty people API
  slug: twenty-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-people-api-openapi.yml
- filename: twenty-relations-api-openapi.yml
  format: yaml
  label: Twenty relations API
  slug: twenty-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-relations-api-openapi.yml
- filename: twenty-tasks-api-openapi.yml
  format: yaml
  label: Twenty tasks API
  slug: twenty-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/openapi/twenty-tasks-api-openapi.yml
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
