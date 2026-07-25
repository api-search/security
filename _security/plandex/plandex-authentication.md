---
api_key_in: []
api_specs:
- filename: plandex-accounts-api-openapi.yml
  format: yaml
  label: Plandex Accounts API
  slug: plandex-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-accounts-api-openapi.yml
- filename: plandex-branches-api-openapi.yml
  format: yaml
  label: Plandex Branches API
  slug: plandex-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-branches-api-openapi.yml
- filename: plandex-context-api-openapi.yml
  format: yaml
  label: Plandex Context API
  slug: plandex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-context-api-openapi.yml
- filename: plandex-conversation-api-openapi.yml
  format: yaml
  label: Plandex Conversation API
  slug: plandex-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-conversation-api-openapi.yml
- filename: plandex-diffs-api-openapi.yml
  format: yaml
  label: Plandex Diffs API
  slug: plandex-diffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-diffs-api-openapi.yml
- filename: plandex-execution-api-openapi.yml
  format: yaml
  label: Plandex Execution API
  slug: plandex-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-execution-api-openapi.yml
- filename: plandex-filemap-api-openapi.yml
  format: yaml
  label: Plandex FileMap API
  slug: plandex-filemap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-filemap-api-openapi.yml
- filename: plandex-health-api-openapi.yml
  format: yaml
  label: Plandex Health API
  slug: plandex-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-health-api-openapi.yml
- filename: plandex-invites-api-openapi.yml
  format: yaml
  label: Plandex Invites API
  slug: plandex-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-invites-api-openapi.yml
- filename: plandex-models-api-openapi.yml
  format: yaml
  label: Plandex Models API
  slug: plandex-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-models-api-openapi.yml
- filename: plandex-orgs-api-openapi.yml
  format: yaml
  label: Plandex Orgs API
  slug: plandex-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-orgs-api-openapi.yml
- filename: plandex-plans-api-openapi.yml
  format: yaml
  label: Plandex Plans API
  slug: plandex-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-plans-api-openapi.yml
- filename: plandex-projects-api-openapi.yml
  format: yaml
  label: Plandex Projects API
  slug: plandex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-projects-api-openapi.yml
- filename: plandex-settings-api-openapi.yml
  format: yaml
  label: Plandex Settings API
  slug: plandex-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-settings-api-openapi.yml
- filename: plandex-users-api-openapi.yml
  format: yaml
  label: Plandex Users API
  slug: plandex-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/openapi/plandex-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plandex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plandex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plandex
provider_slug: plandex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token issued by the Plandex server on sign-in. Used by the CLI/REPL for all authenticated API calls.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/plandex-server-openapi.yml
  type: http
slug: plandex-authentication
source_filename: plandex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plandex-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token issued by the Plandex server on sign-in. Used by the CLI/REPL for\n    all authenticated API calls.\n  sources:\n  - openapi/plandex-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/authentication/plandex-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- AI Coding Agent
- Developer Tools
- Open Source
- CLI
- Terminal
- LLM
- Coding Assistant
- Agents
- Go
- Context Management
- Plans
- Self-Hosted
- REST
---
