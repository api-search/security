---
api_key_in:
- header
api_specs:
- filename: gc-ai-chat-api-openapi.yml
  format: yaml
  label: GC AI Chat API
  slug: gc-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-chat-api-openapi.yml
- filename: gc-ai-files-api-openapi.yml
  format: yaml
  label: GC AI Files API
  slug: gc-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-files-api-openapi.yml
- filename: gc-ai-folders-api-openapi.yml
  format: yaml
  label: GC AI Folders API
  slug: gc-ai-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-folders-api-openapi.yml
- filename: gc-ai-playbooks-api-openapi.yml
  format: yaml
  label: GC AI Playbooks API
  slug: gc-ai-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-playbooks-api-openapi.yml
- filename: gc-ai-profiles-api-openapi.yml
  format: yaml
  label: GC AI Profiles API
  slug: gc-ai-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-profiles-api-openapi.yml
- filename: gc-ai-projects-api-openapi.yml
  format: yaml
  label: GC AI Projects API
  slug: gc-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-projects-api-openapi.yml
- filename: gc-ai-skills-api-openapi.yml
  format: yaml
  label: GC AI Skills API
  slug: gc-ai-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-skills-api-openapi.yml
- filename: gc-ai-usage-api-openapi.yml
  format: yaml
  label: GC AI Usage API
  slug: gc-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-usage-api-openapi.yml
- filename: gc-ai-utility-api-openapi.yml
  format: yaml
  label: GC AI Utility API
  slug: gc-ai-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-utility-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gc Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: GC AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GC AI
provider_slug: gc-ai
scheme_count: 1
schemes:
- description: 'API key for authentication, passed in the Authorization header.

    Create API keys in the GC AI app under Settings → API.'
  in: header
  key_types:
  - access: Only non-access-controlled resources; rejected by user-scoped endpoints (422).
    identity: Represents the whole workspace (system account). Created/revoked by org admins.
    prefix: gcai_
    scope: organization
    use_case: Backend services, scheduled jobs, shared automations.
  - access: Everything the user can read, including privately shared files and projects; works with user-scoped endpoints (e.g. chat search, star/unstar).
    identity: Carries the individual member's identity; requires the org "User API Keys Policy" to be enabled.
    prefix: u:gcai_
    scope: user
    use_case: Individual scripting/analysis where attribution matters.
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/gc-ai-openapi-original.yml
  type: apiKey
slug: gc-ai-authentication
source_filename: gc-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gc-ai-openapi-original.yml\ndocs: https://docs.gc.ai/api-reference/concepts/api-keys\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    API key for authentication, passed in the Authorization header.\n    Create API keys in the GC AI app under Settings → API.\n  key_types:\n  - scope: organization\n    prefix: gcai_\n    identity: Represents the whole workspace (system account). Created/revoked by org admins.\n    access: Only non-access-controlled resources; rejected by user-scoped endpoints (422).\n    use_case: Backend services, scheduled jobs, shared automations.\n  - scope: user\n    prefix: 'u:gcai_'\n    identity: Carries the individual member's identity; requires the org \"User API Keys Policy\" to be enabled.\n    access: Everything the user can read, including privately shared files and projects;\
  \ works with user-scoped endpoints (e.g. chat search, star/unstar).\n    use_case: Individual scripting/analysis where attribution matters.\n  sources:\n  - openapi/gc-ai-openapi-original.yml\nnotes: >-\n  The External API is key-only (no OAuth scopes). GC AI does run an OAuth 2.1\n  authorization server, but only for its MCP server (see mcp/gc-ai-mcp.yml and\n  well-known/gc-ai-oauth-authorization-server.json), not for the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/authentication/gc-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Legal
- Legal AI
- Contracts
- In-House Counsel
- Artificial Intelligence
- Document Review
- Enterprise
- MCP
---
