---
api_key_in: []
api_specs:
- filename: trellistech-public-api.json
  format: json
  label: Trellis Public API
  slug: trellis-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellistech/refs/heads/main/openapi/trellistech-public-api.json
auth_types: []
description: 'Trellis supports two authentication methods for API and MCP access: workspace-scoped API keys for trusted server-side integrations and MCP clients, and programmatic session tokens for email/password flows that run under a specific Trellis user account.'
kind: authentication
layout: security
method: searched
name: Trellistech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellis declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Trellis
provider_slug: trellistech
scheme_count: 2
schemes:
- bearer_format: trls_...
  description: 'Workspace-scoped API key created in Settings > Developer. Sent as `Authorization: Bearer trls_...`. The {workspaceId} path segment must match the workspace that issued the key; cross-workspace calls are rejected with 401.'
  from_openapi: true
  id: WorkspaceApiKey
  location: Authorization header
  properties:
    display: shown once at creation; lost keys must be revoked and recreated
    revocable: revoked keys stop working immediately (clients then receive 401)
    rotation: create separate keys per system so one can be revoked independently
    scope: single workspace per key
    server_side_only: true
  scheme: bearer
  type: http
- bearer_format: JWT access token
  description: Programmatic session token obtained from POST /api/v1/auth/token with email and password. Runs under a specific Trellis user profile. Works at runtime but is NOT reflected in the generated OpenAPI (which documents workspace API keys only).
  endpoints:
  - description: Authenticate with email and password; returns accessToken + refreshToken
    method: POST
    path: /api/v1/auth/token
  - description: Exchange a refresh token for a new access token
    method: POST
    path: /api/v1/auth/refresh
  - description: Get the authenticated user profile (workspace API keys receive 401 here)
    method: GET
    path: /api/v1/auth/me
  from_openapi: false
  id: SessionToken
  scheme: bearer
  token:
    expires_in_seconds: 3600
    refresh: refreshToken via /api/v1/auth/refresh
    type: bearer JWT
  type: http
slug: trellistech-authentication
source_filename: trellistech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.trellistech.com/api-reference/authentication\ndocs: https://docs.trellistech.com/api-reference/authentication\nname: Trellis Public API Authentication\ndescription: >-\n  Trellis supports two authentication methods for API and MCP access: workspace-scoped\n  API keys for trusted server-side integrations and MCP clients, and programmatic session\n  tokens for email/password flows that run under a specific Trellis user account.\nschemes:\n- id: WorkspaceApiKey\n  type: http\n  scheme: bearer\n  bearer_format: trls_...\n  location: Authorization header\n  from_openapi: true\n  description: >-\n    Workspace-scoped API key created in Settings > Developer. Sent as\n    `Authorization: Bearer trls_...`. The {workspaceId} path segment must match the\n    workspace that issued the key; cross-workspace calls are rejected with 401.\n  properties:\n    scope: single workspace per key\n    server_side_only: true\n    revocable:\
  \ revoked keys stop working immediately (clients then receive 401)\n    display: shown once at creation; lost keys must be revoked and recreated\n    rotation: create separate keys per system so one can be revoked independently\n- id: SessionToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT access token\n  from_openapi: false\n  description: >-\n    Programmatic session token obtained from POST /api/v1/auth/token with email and\n    password. Runs under a specific Trellis user profile. Works at runtime but is NOT\n    reflected in the generated OpenAPI (which documents workspace API keys only).\n  endpoints:\n  - method: POST\n    path: /api/v1/auth/token\n    description: Authenticate with email and password; returns accessToken + refreshToken\n  - method: POST\n    path: /api/v1/auth/refresh\n    description: Exchange a refresh token for a new access token\n  - method: GET\n    path: /api/v1/auth/me\n    description: Get the authenticated user profile (workspace API keys receive\
  \ 401 here)\n  token:\n    type: bearer JWT\n    expires_in_seconds: 3600\n    refresh: refreshToken via /api/v1/auth/refresh\noauth2: false\nopenid_connect: false\nmutual_tls: false\nsecurity_best_practices:\n- Store keys and tokens in environment variables or a secret manager; never commit to source control.\n- Rotate keys periodically; create separate keys per system for independent revocation.\n- Require explicit user confirmation before a connected client creates/updates records or sends messages.\n- Store refresh tokens securely and refresh proactively before the access token expires.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellistech/refs/heads/main/authentication/trellistech-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Property Management
- Vacation Rentals
- Short-Term Rentals
- AI Agents
- Operations
- Hospitality
- Task Management
- Model Context Protocol
---
