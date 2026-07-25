---
api_key_in: []
api_specs:
- filename: paragon-proxy-api-openapi.yml
  format: yaml
  label: Proxy API
  slug: proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-proxy-api-openapi.yml
- filename: paragon-users-api-openapi.yml
  format: yaml
  label: Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-users-api-openapi.yml
- filename: paragon-task-history-api-openapi.yml
  format: yaml
  label: Task History API
  slug: task-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-task-history-api-openapi.yml
- filename: paragon-triggers-api-openapi.yml
  format: yaml
  label: Triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-triggers-api-openapi.yml
- filename: paragon-credentials-api-openapi.yml
  format: yaml
  label: Paragon Credentials API
  slug: paragon-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-credentials-api-openapi.yml
- filename: paragon-custom-integrations-api-openapi.yml
  format: yaml
  label: Paragon Custom Integrations API
  slug: paragon-custom-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-custom-integrations-api-openapi.yml
- filename: paragon-integrations-api-openapi.yml
  format: yaml
  label: Paragon Integrations API
  slug: paragon-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-integrations-api-openapi.yml
- filename: paragon-permissions-api-openapi.yml
  format: yaml
  label: Paragon Permissions API
  slug: paragon-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-permissions-api-openapi.yml
- filename: paragon-sync-api-openapi.yml
  format: yaml
  label: Paragon Sync API
  slug: paragon-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-sync-api-openapi.yml
- filename: paragon-tools-api-openapi.yml
  format: yaml
  label: Paragon Tools API
  slug: paragon-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-tools-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paragon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paragon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paragon
provider_slug: paragon
scheme_count: 1
schemes:
- description: Paragon User Token. A signed JWT token used to authenticate a Connected User.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paragon-actionkit-api-openapi.yml
  - openapi/paragon-managed-sync-api-openapi.yml
  - openapi/paragon-proxy-api-openapi.yml
  - openapi/paragon-task-history-api-openapi.yml
  - openapi/paragon-triggers-api-openapi.yml
  - openapi/paragon-users-api-openapi.yml
  type: http
slug: paragon-authentication
source_filename: paragon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paragon-actionkit-api-openapi.yml, openapi/paragon-managed-sync-api-openapi.yml,\n  openapi/paragon-proxy-api-openapi.yml, openapi/paragon-task-history-api-openapi.yml, openapi/paragon-triggers-api-openapi.yml,\n  openapi/paragon-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Paragon User Token. A signed JWT token used to authenticate a Connected User.\n  sources:\n  - openapi/paragon-actionkit-api-openapi.yml\n  - openapi/paragon-managed-sync-api-openapi.yml\n  - openapi/paragon-proxy-api-openapi.yml\n  - openapi/paragon-task-history-api-openapi.yml\n  - openapi/paragon-triggers-api-openapi.yml\n  - openapi/paragon-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/authentication/paragon-authentication.yml
summary_line: http · 1 scheme
tags:
- Embedded Integrations
- Integration Infrastructure
- iPaaS
- AI Agents
- MCP
- Integrations
---
