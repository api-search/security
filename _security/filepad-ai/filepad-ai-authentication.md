---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filepad-ai-openapi-generated.yml
  format: yaml
  label: Filepad API
  slug: filepad-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filepad-ai/openapi/_ae-authored/filepad-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Filepad Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filepad declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Filepad
provider_slug: filepad-ai
scheme_count: 1
schemes:
- description: 'Agent Access API v1 requires OAuth 2.1 bearer tokens. Unauthenticated requests receive a WWW-Authenticate: Bearer challenge plus the OAuth metadata URL. Tokens are workspace-scoped and carry only explicitly granted scopes.'
  header: Authorization
  location: header
  name: bearer
  scheme: Bearer
  type: oauth2
slug: filepad-ai-authentication
source_filename: filepad-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filepad.ai/docs/integrations/api-v1/\ndocs: https://filepad.ai/docs/security/overview/\nschemes:\n  - type: oauth2\n    name: bearer\n    description: >-\n      Agent Access API v1 requires OAuth 2.1 bearer tokens. Unauthenticated\n      requests receive a WWW-Authenticate: Bearer challenge plus the OAuth\n      metadata URL. Tokens are workspace-scoped and carry only explicitly\n      granted scopes.\n    location: header\n    header: Authorization\n    scheme: Bearer\nnotes: >-\n  Agent Access keys are workspace-scoped; a key for one workspace cannot access\n  another. Keys can be created, secret-rotated, scope-patched, and revoked by\n  workspace admins from the Agents panel. The native FilepadAI run API\n  (/agent/...) uses in-app session auth, not Agent Access keys. The MCP\n  endpoint (/mcp) uses the same OAuth bearer tokens with its own scope set.\n"
source_yaml_url: https://artifacts.apis.io/filepad-ai/authentication/filepad-ai-authentication.yml
summary_line: 1 scheme
tags:
- Low-Code
- No-Code
- AI Agents
- Workflows
- Developer Tools
- Internal Tools
- Workspace
- Apps
---
