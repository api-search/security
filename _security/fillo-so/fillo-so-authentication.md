---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fillo-so-agents-api-openapi.yml
  format: yaml
  label: Fillo Agents API
  slug: fillo-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-agents-api-openapi.yml
- filename: fillo-so-credentials-api-openapi.yml
  format: yaml
  label: Fillo Credentials API
  slug: fillo-so-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-credentials-api-openapi.yml
- filename: fillo-so-deliveries-api-openapi.yml
  format: yaml
  label: Fillo Deliveries API
  slug: fillo-so-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-deliveries-api-openapi.yml
- filename: fillo-so-fillo-management-api-api-openapi.yml
  format: yaml
  label: Fillo Fillo Management API
  slug: fillo-so-fillo-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-fillo-management-api-api-openapi.yml
- filename: fillo-so-forms-api-openapi.yml
  format: yaml
  label: Fillo Forms API
  slug: fillo-so-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-forms-api-openapi.yml
- filename: fillo-so-insights-api-openapi.yml
  format: yaml
  label: Fillo Insights API
  slug: fillo-so-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-insights-api-openapi.yml
- filename: fillo-so-integrations-api-openapi.yml
  format: yaml
  label: Fillo Integrations API
  slug: fillo-so-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-integrations-api-openapi.yml
- filename: fillo-so-members-api-openapi.yml
  format: yaml
  label: Fillo Members API
  slug: fillo-so-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-members-api-openapi.yml
- filename: fillo-so-respondents-api-openapi.yml
  format: yaml
  label: Fillo Respondents API
  slug: fillo-so-respondents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-respondents-api-openapi.yml
- filename: fillo-so-responses-api-openapi.yml
  format: yaml
  label: Fillo Responses API
  slug: fillo-so-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-responses-api-openapi.yml
- filename: fillo-so-settings-api-openapi.yml
  format: yaml
  label: Fillo Settings API
  slug: fillo-so-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-settings-api-openapi.yml
- filename: fillo-so-storage-api-openapi.yml
  format: yaml
  label: Fillo Storage API
  slug: fillo-so-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-storage-api-openapi.yml
- filename: fillo-so-webhooks-api-openapi.yml
  format: yaml
  label: Fillo Webhooks API
  slug: fillo-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-webhooks-api-openapi.yml
- filename: fillo-so-workspace-api-openapi.yml
  format: yaml
  label: Fillo Workspace API
  slug: fillo-so-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-workspace-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fillo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fillo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fillo
provider_slug: fillo-so
scheme_count: 2
schemes:
- description: 'Project secret keys of the form `fsk_…` (bearer tokens) authenticate every Management

    API call to https://fillo.so/api/v1/manage. Create a key in the dashboard under

    Settings → Connections → API keys, or with `fillo keys create --preset read|agent|full`.

    The plaintext is shown once; Fillo stores only its hash. Keys carry an explicit set

    of scopes — a request for a scope the key lacks returns 403 with a stable message

    naming the missing scope. 401 is returned for missing, malformed, unknown, revoked,

    or expired keys. Management routes are not CORS-open, so a key pasted into browser

    code fails fast; keep `fsk_` keys server-side.

    '
  name: bearerAuth
  scheme: bearer
  sources:
  - https://fillo.so/docs/api
  - openapi/fillo-so-openapi.json
  type: http
- description: 'The remote MCP server at https://fillo.so/api/mcp is OAuth 2.1 with S256 PKCE and

    RFC 7591 Dynamic Client Registration. Clients discover authorization from

    https://fillo.so/.well-known/oauth-protected-resource. Approving consent on

    fillo.so mints a backing project key that appears in the keys list as

    "MCP: <client>" and can be revoked there at any time.

    '
  flow: authorization_code
  name: oauth2_mcp
  sources:
  - https://fillo.so/docs/api
  - https://fillo.so/.well-known/oauth-protected-resource
  type: oauth2
slug: fillo-so-authentication
source_filename: fillo-so-authentication.yml
source_heading: Authentication Profile
source_url: https://fillo.so/docs/api
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fillo.so/docs/api\nsources:\n- https://fillo.so/docs/api\n- https://fillo.so/docs/security\n- openapi/fillo-so-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\ndocs: https://fillo.so/docs/api#auth\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |\n    Project secret keys of the form `fsk_…` (bearer tokens) authenticate every Management\n    API call to https://fillo.so/api/v1/manage. Create a key in the dashboard under\n    Settings → Connections → API keys, or with `fillo keys create --preset read|agent|full`.\n    The plaintext is shown once; Fillo stores only its hash. Keys carry an explicit set\n    of scopes — a request for a scope the key lacks returns 403 with a stable message\n    naming the missing scope. 401 is returned for missing, malformed, unknown, revoked,\n    or expired keys. Management routes are not CORS-open, so a key pasted into browser\n    code fails fast;\
  \ keep `fsk_` keys server-side.\n  sources:\n  - https://fillo.so/docs/api\n  - openapi/fillo-so-openapi.json\n- name: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  description: |\n    The remote MCP server at https://fillo.so/api/mcp is OAuth 2.1 with S256 PKCE and\n    RFC 7591 Dynamic Client Registration. Clients discover authorization from\n    https://fillo.so/.well-known/oauth-protected-resource. Approving consent on\n    fillo.so mints a backing project key that appears in the keys list as\n    \"MCP: <client>\" and can be revoked there at any time.\n  sources:\n  - https://fillo.so/docs/api\n  - https://fillo.so/.well-known/oauth-protected-resource\nother_credentials:\n- name: publishable_key\n  prefix: pk_\n  description: Project publishable key — syncs code-defined schemas into one project from client code. Cannot read responses or manage the workspace. Safe in a client bundle; constrained by project allowed-origins.\n- name: cli_token\n  prefix: fcli_\n  description:\
  \ Private CLI/Zapier token — full management access bound to the minting user and project while workspace owner/admin authority remains. Plaintext shown once; Fillo stores a hash.\n- name: identity_secret\n  prefix: is_\n  description: Server-side HMAC key for signing respondent external IDs and profile fields; protects respondent attribution. Never expose to the browser.\n- name: webhook_signing_secret\n  description: Per-webhook HMAC-SHA256 secret shown once at creation; used to verify X-Fillo-Signature on each delivery.\n- name: sync_token\n  description: Stage-only token used by the CLI for code-defined form sync. Returned exactly once by POST /api/v1/manage/sync-tokens.\n"
source_yaml_url: https://artifacts.apis.io/fillo-so/authentication/fillo-so-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Forms
- Form Builder
- Developer Tools
- Embeddable Widgets
- Webhook
- Validation
- File Uploads
- SDK
- CLI
- Management API
---
