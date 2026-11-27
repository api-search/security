---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: craaft-io-attachments-api-openapi.yml
  format: yaml
  label: craaft Attachments API
  slug: craaft-io-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-attachments-api-openapi.yml
- filename: craaft-io-board-templates-api-openapi.yml
  format: yaml
  label: craaft Board Templates API
  slug: craaft-io-board-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-board-templates-api-openapi.yml
- filename: craaft-io-cards-api-openapi.yml
  format: yaml
  label: craaft Cards API
  slug: craaft-io-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-cards-api-openapi.yml
- filename: craaft-io-checklist-api-openapi.yml
  format: yaml
  label: craaft Checklist API
  slug: craaft-io-checklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-checklist-api-openapi.yml
- filename: craaft-io-columns-api-openapi.yml
  format: yaml
  label: craaft Columns API
  slug: craaft-io-columns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-columns-api-openapi.yml
- filename: craaft-io-comments-api-openapi.yml
  format: yaml
  label: craaft Comments API
  slug: craaft-io-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-comments-api-openapi.yml
- filename: craaft-io-imports-api-openapi.yml
  format: yaml
  label: craaft Imports API
  slug: craaft-io-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-imports-api-openapi.yml
- filename: craaft-io-invitations-api-openapi.yml
  format: yaml
  label: craaft Invitations API
  slug: craaft-io-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-invitations-api-openapi.yml
- filename: craaft-io-me-api-openapi.yml
  format: yaml
  label: craaft Me API
  slug: craaft-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-me-api-openapi.yml
- filename: craaft-io-members-api-openapi.yml
  format: yaml
  label: craaft Members API
  slug: craaft-io-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-members-api-openapi.yml
- filename: craaft-io-milestones-api-openapi.yml
  format: yaml
  label: craaft Milestones API
  slug: craaft-io-milestones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-milestones-api-openapi.yml
- filename: craaft-io-projects-api-openapi.yml
  format: yaml
  label: craaft Projects API
  slug: craaft-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-projects-api-openapi.yml
- filename: craaft-io-public-api-openapi.yml
  format: yaml
  label: craaft Public API
  slug: craaft-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-public-api-openapi.yml
- filename: craaft-io-search-api-openapi.yml
  format: yaml
  label: craaft Search API
  slug: craaft-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-search-api-openapi.yml
- filename: craaft-io-users-api-openapi.yml
  format: yaml
  label: craaft Users API
  slug: craaft-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-users-api-openapi.yml
- filename: craaft-io-version-api-openapi.yml
  format: yaml
  label: craaft Version API
  slug: craaft-io-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-version-api-openapi.yml
- filename: craaft-io-webhooks-api-openapi.yml
  format: yaml
  label: craaft Webhooks API
  slug: craaft-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: craaft Authentication
name_suffix: Authentication
oauth_flows: []
overview: craaft secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: craaft
provider_slug: craaft-io
scheme_count: 2
schemes:
- description: 'Browser session cookie (`__Host-craaft_session` in production,

    `craaft_session` in dev), set at sign-in. Not obtainable through

    this API - it''s here only so the handful of session-only routes

    below (the OAuth consent screen''s own endpoints, connected-apps

    management) can be marked accurately. They reject both bearer

    schemes with a 403.'
  in: cookie
  name: sessionAuth
  parameter: craaft_session
  sources:
  - openapi/craaft-io-openapi.yml
  type: apiKey
- bearerFormat: cra_<24 base64url chars>
  description: 'Two token schemes, same permissions. `cra_<24 base64url chars>` is a

    personal access token minted in Settings, doesn''t expire on its own,

    and is revoked from the same page. `cro_<32 base64url chars>` is an

    OAuth access token issued to an OAuth client (an MCP client such as

    Claude) via the authorization-code-with-PKCE flow; it expires after

    1 hour and the client refreshes it. Either token authentic'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/craaft-io-openapi.yml
  type: http
slug: craaft-io-authentication
source_filename: craaft-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://craaft.io/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: craaft_session\n  description: 'Browser session cookie (`__Host-craaft_session` in production,\n\n    `craaft_session` in dev), set at sign-in. Not obtainable through\n\n    this API - it''s here only so the handful of session-only routes\n\n    below (the OAuth consent screen''s own endpoints, connected-apps\n\n    management) can be marked accurately. They reject both bearer\n\n    schemes with a 403.'\n  sources:\n  - openapi/craaft-io-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: cra_<24 base64url chars>\n  description: 'Two token schemes, same permissions. `cra_<24 base64url chars>` is a\n\n    personal access token minted in Settings, doesn''t expire on its own,\n\n    and is revoked from the same page. `cro_<32 base64url\
  \ chars>` is an\n\n    OAuth access token issued to an OAuth client (an MCP client such as\n\n    Claude) via the authorization-code-with-PKCE flow; it expires after\n\n    1 hour and the client refreshes it. Either token authentic'\n  sources:\n  - openapi/craaft-io-openapi.yml\ndocs: https://craaft.io/docs\ndocs_notes:\n- Base URL https://craaft.io/api/v1 . The version prefix is mandatory, and unversioned paths return 404.\n- 'Header Authorization: Bearer cra_... on every request. The scheme is case-insensitive. Personal tokens start with cra_ ; tokens an MCP client gets from signing in start with cro_ .'\n- Sign-in, API key management, billing and avatar upload stay session-only.\n- Docs say tokens are \"cra_ followed by 32 characters\"; the spec bearerFormat says cra_<24 base64url chars> - the two disagree on length.\n- OAuth 2.1 with PKCE for MCP clients; endpoints discovered at /.well-known/oauth-authorization-server (RFC 8414), per the spec bearerAuth description and https://craaft.io/mcp.\n"
source_yaml_url: https://artifacts.apis.io/craaft-io/authentication/craaft-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Task Management
- Kanban
- Project Management
- Productivity
- AI Agents
- MCP
- REST API
- Collaboration
---
