---
api_key_in: []
api_specs:
- filename: loops-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-api-key-api-openapi.yml
- filename: loops-audience-segments-api-openapi.yml
  format: yaml
  label: Loops Audience segments API
  slug: loops-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-audience-segments-api-openapi.yml
- filename: loops-campaign-groups-api-openapi.yml
  format: yaml
  label: Loops Campaign groups API
  slug: loops-campaign-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaign-groups-api-openapi.yml
- filename: loops-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaigns-api-openapi.yml
- filename: loops-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-components-api-openapi.yml
- filename: loops-configuration-api-openapi.yml
  format: yaml
  label: Loops Configuration API
  slug: loops-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-configuration-api-openapi.yml
- filename: loops-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contact-properties-api-openapi.yml
- filename: loops-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contacts-api-openapi.yml
- filename: loops-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-email-messages-api-openapi.yml
- filename: loops-event-patterns-api-openapi.yml
  format: yaml
  label: Loops Event patterns API
  slug: loops-event-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-event-patterns-api-openapi.yml
- filename: loops-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-events-api-openapi.yml
- filename: loops-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-mailing-lists-api-openapi.yml
- filename: loops-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-themes-api-openapi.yml
- filename: loops-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-emails-api-openapi.yml
- filename: loops-transactional-groups-api-openapi.yml
  format: yaml
  label: Loops Transactional groups API
  slug: loops-transactional-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-groups-api-openapi.yml
- filename: loops-uploads-api-openapi.yml
  format: yaml
  label: Loops Uploads API
  slug: loops-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-uploads-api-openapi.yml
- filename: loops-workflow-nodes-api-openapi.yml
  format: yaml
  label: Loops Workflow nodes API
  slug: loops-workflow-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflow-nodes-api-openapi.yml
- filename: loops-workflows-api-openapi.yml
  format: yaml
  label: Loops Workflows API
  slug: loops-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflows-api-openapi.yml
- filename: loops-webhooks-asyncapi.yml
  format: yaml
  label: Loops Webhooks
  slug: loops-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/asyncapi/loops-webhooks-asyncapi.yml
- filename: loops-webhooks-api-openapi.yml
  format: yaml
  label: Loops Webhooks API
  slug: loops-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Loops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loops secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loops
provider_slug: loops
scheme_count: 2
schemes:
- applied_to: '64 of 64 operations (per-operation `security: [{apiKey: []}]`)'
  constraints:
  - Must never be used client side or exposed to end users.
  - CORS is not supported — the API rejects cross-origin browser requests by design, so the key can only be used server side.
  - A key is bound to one team. Multi-team automation needs one key per team; the CLI models this directly with named keyring entries and a `--team` flag.
  expiring: false
  failure_body: '{ "success": false, "message": "Invalid API key" }'
  failure_status: 401
  format: Bearer <api-key>
  header: Authorization
  name: apiKey
  provisioning: Settings -> API in the Loops app (https://app.loops.so/settings?page=api), "Generate key". Keys can be named and revoked individually; Loops recommends a separate key per purpose.
  rotatable: true
  scheme: bearer
  scoped: false
  sources:
  - openapi/_original/loops-openapi.yaml
  - https://loops.so/docs/api-reference/intro
  surface: REST API
  type: http
  validation_endpoint:
    note: A dedicated, cheap, non-mutating endpoint for verifying a credential and discovering which team it belongs to. Also exposed as `loops api-key` in the CLI.
    operationId: testApiKey
    path: GET /v1/api-key
    returns: '{ "success": true, "teamName": "..." }'
- authorization_endpoint: https://app.loops.so/oauth/authorize
  challenge: 'An unauthenticated call to the MCP endpoint returns 401 with `WWW-Authenticate: Bearer resource_metadata="https://mcp.loops.so/.well-known/oauth-protected-resource", scope="mcp"`.'
  client_authentication: none (public client)
  client_registration: Client ID Metadata Documents, or pre-registration with Loops. No RFC 7591 DCR.
  discovery:
    authorization_server_metadata: https://app.loops.so/.well-known/oauth-authorization-server
    protected_resource_metadata: https://mcp.loops.so/.well-known/oauth-protected-resource
  flow: authorization_code
  issuer: https://app.loops.so
  name: oauth2
  pkce: required (S256)
  refresh_tokens: true
  revocation_endpoint: https://app.loops.so/oauth/revoke
  scopes:
  - mcp
  sources:
  - https://app.loops.so/.well-known/oauth-authorization-server
  - https://mcp.loops.so/.well-known/oauth-protected-resource
  - https://loops.so/docs/mcp-server
  surface: MCP server (https://mcp.loops.so)
  token_endpoint: https://app.loops.so/oauth/token
  type: oauth2
slug: loops-authentication
source_filename: loops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://loops.so/docs/api-reference/intro\ndocs:\n  rest: https://loops.so/docs/api-reference/intro\n  cli: https://loops.so/docs/cli\n  mcp: https://loops.so/docs/mcp-server\nderived_from: openapi/_original/loops-openapi.yaml (1.21.6)\nsummary:\n  types:\n    - http\n    - oauth2\n  note: >-\n    Two separate authentication systems that do not overlap. The REST API is\n    bearer API key, unscoped, one key per team. The MCP server is OAuth 2.0\n    authorization code with PKCE, one scope. An API key cannot be used against\n    the MCP server and an OAuth token cannot be used against the REST API.\nschemes:\n  - name: apiKey\n    type: http\n    scheme: bearer\n    surface: REST API\n    header: Authorization\n    format: 'Bearer <api-key>'\n    applied_to: '64 of 64 operations (per-operation `security: [{apiKey: []}]`)'\n    scoped: false\n    expiring: false\n    rotatable: true\n    provisioning: >-\n      Settings -> API\
  \ in the Loops app (https://app.loops.so/settings?page=api),\n      \"Generate key\". Keys can be named and revoked individually; Loops\n      recommends a separate key per purpose.\n    validation_endpoint:\n      operationId: testApiKey\n      path: GET /v1/api-key\n      returns: '{ \"success\": true, \"teamName\": \"...\" }'\n      note: >-\n        A dedicated, cheap, non-mutating endpoint for verifying a credential and\n        discovering which team it belongs to. Also exposed as `loops api-key` in\n        the CLI.\n    failure_status: 401\n    failure_body: '{ \"success\": false, \"message\": \"Invalid API key\" }'\n    constraints:\n      - Must never be used client side or exposed to end users.\n      - >-\n        CORS is not supported — the API rejects cross-origin browser requests by\n        design, so the key can only be used server side.\n      - >-\n        A key is bound to one team. Multi-team automation needs one key per\n        team; the CLI models this directly\
  \ with named keyring entries and a\n        `--team` flag.\n    sources:\n      - openapi/_original/loops-openapi.yaml\n      - https://loops.so/docs/api-reference/intro\n  - name: oauth2\n    type: oauth2\n    surface: MCP server (https://mcp.loops.so)\n    flow: authorization_code\n    pkce: required (S256)\n    scopes:\n      - mcp\n    issuer: https://app.loops.so\n    authorization_endpoint: https://app.loops.so/oauth/authorize\n    token_endpoint: https://app.loops.so/oauth/token\n    revocation_endpoint: https://app.loops.so/oauth/revoke\n    refresh_tokens: true\n    client_authentication: none (public client)\n    client_registration: Client ID Metadata Documents, or pre-registration with Loops. No RFC 7591 DCR.\n    discovery:\n      authorization_server_metadata: https://app.loops.so/.well-known/oauth-authorization-server\n      protected_resource_metadata: https://mcp.loops.so/.well-known/oauth-protected-resource\n    challenge: >-\n      An unauthenticated call to the MCP\
  \ endpoint returns 401 with\n      `WWW-Authenticate: Bearer resource_metadata=\"https://mcp.loops.so/.well-known/oauth-protected-resource\", scope=\"mcp\"`.\n    sources:\n      - https://app.loops.so/.well-known/oauth-authorization-server\n      - https://mcp.loops.so/.well-known/oauth-protected-resource\n      - https://loops.so/docs/mcp-server\ncli_credential_handling:\n  storage: OS keyring, multiple named team keys\n  env_var: LOOPS_API_KEY\n  precedence:\n    - LOOPS_API_KEY\n    - --team flag\n    - stored default (`loops auth use`)\nwebhook_authentication:\n  direction: inbound to subscriber\n  mechanism: HMAC-SHA256 signature, Standard-Webhooks-style headers\n  headers:\n    - webhook-id\n    - webhook-timestamp\n    - webhook-signature\n  secret: issued per endpoint at https://app.loops.so/settings?page=webhooks, prefixed `whsec_`\n  see: asyncapi/loops-webhooks-asyncapi.yml\ngaps:\n  - No scoped or least-privilege REST credentials — every API key is full-access for its team.\n\
  \  - No key expiry or automatic rotation; rotation is manual.\n  - No OAuth path for third-party applications against the REST API; OAuth exists only for MCP.\n  - No mTLS, no request signing, no IP allowlisting documented.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/authentication/loops-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Email
- Email API
- Marketing Automation
- Transactional Email
- Lifecycle Email
- Webhook
- Software-as-a-Service
- Communications
- Developer Tools
- MCP
- Agents
- Campaigns
---
