---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: configure-dev-auth-api-openapi.yml
  format: yaml
  label: Configure Auth API
  slug: configure-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-auth-api-openapi.yml
- filename: configure-dev-connectors-api-openapi.yml
  format: yaml
  label: Configure Connectors API
  slug: configure-dev-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-connectors-api-openapi.yml
- filename: configure-dev-files-api-openapi.yml
  format: yaml
  label: Configure Files API
  slug: configure-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-files-api-openapi.yml
- filename: configure-dev-import-api-openapi.yml
  format: yaml
  label: Configure Import API
  slug: configure-dev-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-import-api-openapi.yml
- filename: configure-dev-profile-api-openapi.yml
  format: yaml
  label: Configure Profile API
  slug: configure-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-profile-api-openapi.yml
- filename: configure-dev-web-api-openapi.yml
  format: yaml
  label: Configure Web API
  slug: configure-dev-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-web-api-openapi.yml
- filename: configure-dev-webhooks-api-openapi.yml
  format: yaml
  label: Configure Webhooks API
  slug: configure-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Configure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Configure secures its APIs with apiKey, http, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Configure
provider_slug: configure-dev
scheme_count: 6
schemes:
- description: Configure API key. Use sk_ on servers. pk_ is browser-safe but restricted.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/configure-dev-openapi.yml
  - https://docs.configure.dev/reference/api.md
  type: apiKey
- description: Your agent handle; sent on every server-side request (documented, not a securityScheme in the spec).
  in: header
  name: AgentHeader
  parameter: X-Agent
  sources:
  - https://docs.configure.dev/reference/api.md
  type: apiKey
- bearerFormat: JWT
  description: Agent-scoped Configure token from sign-in / hosted Configure.link().
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/configure-dev-openapi.yml
  type: http
- description: Stable external user ID for unlinked developer-scoped profiles. Requires sk_. Linked users who have not approved the agent get 403 approval_required.
  in: header
  name: ExternalUserId
  parameter: X-User-Id
  sources:
  - openapi/configure-dev-openapi.yml
  - https://docs.configure.dev/reference/api.md
  type: apiKey
- description: Sign in with Configure over OpenID Connect. Authorization code + PKCE (S256) at https://api.configure.dev/oauth/authorize, code exchange at POST /oauth/token; scopes openid email profile; client ids carry the oc_ prefix. Code lasts 5 minutes and works once; access token lasts 1 hour; refresh token issued.
  name: ConfigureOIDC
  sources:
  - https://docs.configure.dev/oidc.md
  type: openIdConnect
- description: Remote MCP server https://mcp.configure.dev; the MCP client handles OAuth discovery and PKCE. Tokens carry profile.read profile.search profile.remember profile.commit scopes.
  flow: authorizationCode
  name: MCPOAuth
  sources:
  - https://docs.configure.dev/mcp/overview.md
  - https://docs.configure.dev/oidc.md
  type: oauth2
slug: configure-dev-authentication
source_filename: configure-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.configure.dev/reference/api.md\ndocs: https://docs.configure.dev/reference/api.md\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  note: 'Every server-side request carries X-API-Key (secret key, sk_ prefix, server only) and X-Agent (agent handle). A per-user request also identifies the user with Authorization: Bearer (token from sign-in) or X-User-Id (your own id). pk_ publishable keys are browser-safe. sk_test_/pk_test_ keys address the test plane.'\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Configure API key. Use sk_ on servers. pk_ is browser-safe but restricted.\n  sources:\n  - openapi/configure-dev-openapi.yml\n  - https://docs.configure.dev/reference/api.md\n- name: AgentHeader\n  type: apiKey\n  in: header\n  parameter: X-Agent\n  description: Your agent handle; sent on every server-side request\
  \ (documented, not a securityScheme in the spec).\n  sources:\n  - https://docs.configure.dev/reference/api.md\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Agent-scoped Configure token from sign-in / hosted Configure.link().\n  sources:\n  - openapi/configure-dev-openapi.yml\n- name: ExternalUserId\n  type: apiKey\n  in: header\n  parameter: X-User-Id\n  description: Stable external user ID for unlinked developer-scoped profiles. Requires sk_. Linked users who have not approved the agent get 403 approval_required.\n  sources:\n  - openapi/configure-dev-openapi.yml\n  - https://docs.configure.dev/reference/api.md\n- name: ConfigureOIDC\n  type: openIdConnect\n  description: Sign in with Configure over OpenID Connect. Authorization code + PKCE (S256) at https://api.configure.dev/oauth/authorize, code exchange at POST /oauth/token; scopes openid email profile; client ids carry the oc_ prefix. Code lasts 5 minutes and works once; access token lasts\
  \ 1 hour; refresh token issued.\n  sources:\n  - https://docs.configure.dev/oidc.md\n- name: MCPOAuth\n  type: oauth2\n  flow: authorizationCode\n  description: Remote MCP server https://mcp.configure.dev; the MCP client handles OAuth discovery and PKCE. Tokens carry profile.read profile.search profile.remember profile.commit scopes.\n  sources:\n  - https://docs.configure.dev/mcp/overview.md\n  - https://docs.configure.dev/oidc.md\n"
source_yaml_url: https://artifacts.apis.io/configure-dev/authentication/configure-dev-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 6 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Memory
- Personalization
- User Context
- MCP
---
