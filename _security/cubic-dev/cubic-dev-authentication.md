---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cubic-dev-analytics-api-openapi.yml
  format: yaml
  label: cubic Analytics API
  slug: cubic-dev-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cubic-dev/openapi/cubic-dev-analytics-api-openapi.yml
- filename: cubic-dev-organizations-api-openapi.yml
  format: yaml
  label: cubic Organizations API
  slug: cubic-dev-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cubic-dev/openapi/cubic-dev-organizations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: cubic Authentication
name_suffix: Authentication
oauth_flows: []
overview: cubic secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cubic
provider_slug: cubic-dev
scheme_count: 2
schemes:
- description: One key works for both the Members and Analytics APIs. Personal keys start with cbk_ and use the key owner's organization access; organization keys start with cok_, are created by an organization admin with Read or Admin access, and reach only their own organization. A Read organization key gets 403 admin_required on PATCH. Analytics keys starting with cak_ keep working with the Analytics API but are no longer created. cubic shows the full key value only once.
  format: 'Authorization: Bearer cbk_your_api_key'
  header: Authorization
  issued_at: https://www.cubic.dev/settings?tab=api-cli
  key_prefixes:
  - kind: personal
    prefix: cbk_
  - kind: organization (read or admin)
    prefix: cok_
  - kind: legacy analytics key (Analytics API only, no longer issued)
    prefix: cak_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/cubic-dev-openapi.yml
  - openapi/cubic-dev-analytics-openapi.yml
  - https://docs.cubic.dev/api-reference/overview.md
  type: http
- applies_to: MCP server https://www.cubic.dev/api/mcp
  description: The MCP server is connected by signing in with a cubic account from the MCP client; the docs warn that some clients compare the protected resource URL exactly, so use https://www.cubic.dev/api/mcp rather than https://cubic.dev/api/mcp. Not a REST API scheme.
  name: mcp-oauth
  sources:
  - https://docs.cubic.dev/ide/mcp-server.md
  type: oauth2
slug: cubic-dev-authentication
source_filename: cubic-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cubic.dev/account/members-api\ndocs: https://docs.cubic.dev/account/members-api\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer cbk_your_api_key'\n  description: One key works for both the Members and Analytics APIs. Personal keys start with cbk_ and\n    use the key owner's organization access; organization keys start with cok_, are created by an organization\n    admin with Read or Admin access, and reach only their own organization. A Read organization key gets\n    403 admin_required on PATCH. Analytics keys starting with cak_ keep working with the Analytics API\n    but are no longer created. cubic shows the full key value only once.\n  key_prefixes:\n  - prefix: cbk_\n    kind: personal\n  - prefix: cok_\n    kind: organization (read or admin)\n  - prefix: cak_\n    kind: legacy analytics key (Analytics API\
  \ only, no longer issued)\n  issued_at: https://www.cubic.dev/settings?tab=api-cli\n  sources:\n  - openapi/cubic-dev-openapi.yml\n  - openapi/cubic-dev-analytics-openapi.yml\n  - https://docs.cubic.dev/api-reference/overview.md\n- name: mcp-oauth\n  type: oauth2\n  applies_to: MCP server https://www.cubic.dev/api/mcp\n  description: The MCP server is connected by signing in with a cubic account from the MCP client; the\n    docs warn that some clients compare the protected resource URL exactly, so use https://www.cubic.dev/api/mcp\n    rather than https://cubic.dev/api/mcp. Not a REST API scheme.\n  sources:\n  - https://docs.cubic.dev/ide/mcp-server.md\nkey_types:\n- name: Personal key\n  prefix: cbk_\n  issued_to: Any cubic user\n  acts_as: You, with your own cubic access.\n- name: Organization key\n  prefix: cok_\n  issued_to: An organization admin\n  acts_as: One organization, with read or admin access to its members.\n  access_levels:\n  - Read\n  - Admin\nheader: 'Authorization:\
  \ Bearer cbk_your_api_key'\nnotes:\n- Keys are shown in full only once; the same personal key is used by the CLI (CUBIC_API_KEY), MCP server,\n  Members API and Analytics API.\n- A Read organization key gets 403 admin_required on PATCH. No key can change billing.\n- Legacy cak_ Analytics API keys keep working but are no longer issued.\n"
source_yaml_url: https://artifacts.apis.io/cubic-dev/authentication/cubic-dev-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Code Review
- Developer Tools
- GitHub
- Pull Requests
- MCP
- Analytics
---
