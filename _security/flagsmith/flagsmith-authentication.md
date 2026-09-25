---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-environments-api-openapi.yml
  format: yaml
  label: flagsmith Environments API
  slug: flagsmith-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-environments-api-openapi.yml
- filename: flagsmith-features-api-openapi.yml
  format: yaml
  label: flagsmith Features API
  slug: flagsmith-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-features-api-openapi.yml
- filename: flagsmith-identities-api-openapi.yml
  format: yaml
  label: flagsmith Identities API
  slug: flagsmith-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-identities-api-openapi.yml
- filename: flagsmith-organisations-api-openapi.yml
  format: yaml
  label: flagsmith Organisations API
  slug: flagsmith-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-organisations-api-openapi.yml
- filename: flagsmith-projects-api-openapi.yml
  format: yaml
  label: flagsmith Projects API
  slug: flagsmith-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-projects-api-openapi.yml
- filename: flagsmith-segments-api-openapi.yml
  format: yaml
  label: flagsmith Segments API
  slug: flagsmith-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-segments-api-openapi.yml
- filename: flagsmith-users-api-openapi.yml
  format: yaml
  label: flagsmith Users API
  slug: flagsmith-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-users-api-openapi.yml
- filename: flagsmith-webhooks-api-openapi.yml
  format: yaml
  label: flagsmith Webhooks API
  slug: flagsmith-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Flagsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flagsmith secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flagsmith
provider_slug: flagsmith
scheme_count: 7
schemes:
- description: Per-environment client-side key, found in the dashboard under the project's Environments tab. Safe to ship in client-side code by design. SDKs set the header for you on initialisation; direct HTTP callers must set it on every request.
  docs: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/flags-api/authentication
  in: header
  name: Environment API Key
  parameter: X-Environment-Key
  secret: false
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: SDK / Flags API (https://edge.api.flagsmith.com)
  type: apiKey
- description: Organisation-level secret token. The `Api-Key ` prefix is required — the header must read `Api-Key ser.abc123…`, not the bare key. Requests act with the permissions of the key's user, so administrator privileges are not required and RBAC still applies.
  docs: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/management-api/authentication
  in: header
  name: Master API Key
  parameter: Authorization
  secret: true
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: Management API (https://api.flagsmith.com/api/v1)
  type: apiKey
  value_format: Api-Key <key>
- description: Django REST Framework token authentication, used by session/user tokens rather than organisation keys.
  in: header
  name: tokenAuth
  parameter: Authorization
  secret: true
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: Management API
  type: apiKey
  value_format: Token <key>
- description: For cohort-sync endpoints called by an external cohort source, such as Amplitude.
  name: Cohort Sync Key
  scheme: bearer
  secret: true
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: Cohort sync webhooks
  type: http
- description: For cohort sources that can only send Basic credentials, such as Mixpanel. The key is the password; the username is ignored.
  name: Cohort Sync Key (Basic)
  scheme: basic
  secret: true
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: Cohort sync webhooks
  type: http
- name: basicAuth
  scheme: basic
  secret: true
  sources:
  - openapi/_original/flagsmith-api-openapi.json
  surface: Management API (legacy/internal)
  type: http
- authorization_server: https://api.flagsmith.com
  description: Not declared anywhere in the OpenAPI — discoverable only from the RFC 8414 document on the API host and the RFC 9728 document on the MCP host. Interactive MCP clients use it to avoid handling an API key at all.
  discovery: https://api.flagsmith.com/.well-known/oauth-authorization-server
  docs: https://docs.flagsmith.com/integrating-with-flagsmith/mcp-server
  dynamic_client_registration: https://api.flagsmith.com/o/register/
  flow: authorization_code
  name: OAuth 2.0
  pkce: S256
  scopes:
  - mcp
  - admin-api
  see: scopes/flagsmith-scopes.yml
  surface: MCP server (https://mcp.flagsmith.com) and Management API
  type: oauth2
slug: flagsmith-authentication
source_filename: flagsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/management-api/authentication,\n  https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/flags-api/authentication,\n  https://docs.flagsmith.com/integrating-with-flagsmith/mcp-server,\n  https://api.flagsmith.com/.well-known/oauth-authorization-server (200), and\n  openapi/_original/flagsmith-api-openapi.json#/components/securitySchemes (six declared schemes).\ndocs: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/\nsupersedes: >-\n  The 2026-09-17 derived pass, which read only the nine split specs in openapi/ and saw a single\n  apiKey scheme. The harvested first-party contract declares six, and OAuth 2.0 is declared in none\n  of them — it is only visible in the .well-known metadata.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2: true\n  mtls: false\n  openid_connect:\
  \ false\nkey_insight: >-\n  Two API surfaces, two different keys, and they are not interchangeable — this is the thing to get\n  right first. The SDK/Flags API on edge.api.flagsmith.com takes a NON-SECRET environment key in\n  X-Environment-Key and is safe in client-side code. The Management API on api.flagsmith.com takes a\n  SECRET organisation key in Authorization with a mandatory `Api-Key ` prefix and must never reach a\n  browser. A third path, OAuth 2.0, exists only for the MCP server and the Management API and is\n  absent from the OpenAPI entirely.\nschemes:\n- name: Environment API Key\n  type: apiKey\n  in: header\n  parameter: X-Environment-Key\n  secret: false\n  surface: SDK / Flags API (https://edge.api.flagsmith.com)\n  description: >-\n    Per-environment client-side key, found in the dashboard under the project's Environments tab.\n    Safe to ship in client-side code by design. SDKs set the header for you on initialisation; direct\n    HTTP callers must set it on every\
  \ request.\n  docs: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/flags-api/authentication\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: Master API Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Api-Key <key>'\n  secret: true\n  surface: Management API (https://api.flagsmith.com/api/v1)\n  description: >-\n    Organisation-level secret token. The `Api-Key ` prefix is required — the header must read\n    `Api-Key ser.abc123…`, not the bare key. Requests act with the permissions of the key's user, so\n    administrator privileges are not required and RBAC still applies.\n  docs: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/management-api/authentication\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Token <key>'\n  secret: true\n  surface: Management API\n  description:\
  \ Django REST Framework token authentication, used by session/user tokens rather than organisation keys.\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: Cohort Sync Key\n  type: http\n  scheme: bearer\n  secret: true\n  surface: Cohort sync webhooks\n  description: For cohort-sync endpoints called by an external cohort source, such as Amplitude.\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: Cohort Sync Key (Basic)\n  type: http\n  scheme: basic\n  secret: true\n  surface: Cohort sync webhooks\n  description: >-\n    For cohort sources that can only send Basic credentials, such as Mixpanel. The key is the\n    password; the username is ignored.\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: basicAuth\n  type: http\n  scheme: basic\n  secret: true\n  surface: Management API (legacy/internal)\n  sources: [openapi/_original/flagsmith-api-openapi.json]\n- name: OAuth 2.0\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n\
  \  scopes: [mcp, admin-api]\n  surface: MCP server (https://mcp.flagsmith.com) and Management API\n  authorization_server: https://api.flagsmith.com\n  discovery: https://api.flagsmith.com/.well-known/oauth-authorization-server\n  dynamic_client_registration: https://api.flagsmith.com/o/register/\n  description: >-\n    Not declared anywhere in the OpenAPI — discoverable only from the RFC 8414 document on the API\n    host and the RFC 9728 document on the MCP host. Interactive MCP clients use it to avoid handling\n    an API key at all.\n  docs: https://docs.flagsmith.com/integrating-with-flagsmith/mcp-server\n  see: scopes/flagsmith-scopes.yml\nsso:\n  note: >-\n    End-user sign-in to the Flagsmith dashboard (not API authentication) supports SAML 2.0, Okta,\n    ADFS, LDAP, Google and GitHub OAuth, plus 2FA. SAML, LDAP and SCIM provisioning are Enterprise;\n    2FA is available from the Start-Up plan.\n  docs: https://docs.flagsmith.com/administration-and-security/access-control/\n \
  \ standards: [SAML 2.0, LDAP, SCIM 2.0]\nauthorization:\n  model: RBAC\n  note: >-\n    Roles, permission groups and per-project/per-environment permissions gate every Management API\n    call; custom roles are Enterprise. 34 operations in the contract are tagged Permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/authentication/flagsmith-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Feature Flags
- Remote Config
- Release Management
- A/B Testing
- Experimentation
- Segmentation
- Developer Tools
- DevOps
- Open Source
- Software-as-a-Service
- MCP
- Agent Ready
---
