---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ploy secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ploy
provider_slug: ploy
scheme_count: 3
schemes:
- description: Workspace-scoped personal access token created in workspace Settings → Developer → API tokens. Read by the CLI on every invocation and never written to disk. Each token is pinned to exactly one workspace; the pin is enforced by the API, not by the client, and a mismatched --workspace/PLOY_WORKSPACE_ID exits 1 with "This API token is scoped to a different workspace".
  expiry:
    check: ploy whoami reports the pinned workspace and remaining days
    default_days: 90
    options_days:
    - 30
    - 90
    - 365
    refresh: false
  failure_modes:
  - exit 3 — "PLOY_API_TOKEN is invalid or expired"
  - exit 3 — "PLOY_API_TOKEN is not workspace-scoped"
  in: env
  issuance: The raw token is shown once, with a copyable `export PLOY_API_TOKEN=…` line. It cannot be retrieved later. Any workspace member can create and view their own tokens; owners and admins can view and revoke every token in the workspace.
  name: PloyApiToken
  parameter: PLOY_API_TOKEN
  rate_limit: 60 requests per minute per token
  restrictions: ploy logout, ploy tokens and ploy token revoke are unavailable while PLOY_API_TOKEN is set (exit code 2). API tokens cannot mint replacement credentials or revoke the browser session that created them.
  scheme: bearer
  scope: workspace
  source: https://docs.ploy.ai/cli/authentication
  token_prefix: sk_ploy_pat_
  type: http
- description: 'API key minted per webhook ingest endpoint in workspace Settings → Webhooks and shown once. Sent as `Authorization: Bearer {apiKey}` on every POST to https://ploy.ai/api/v1/webhook/{endpointSlug}. Requests without a valid key are rejected with 401. Disabling or rotating an endpoint invalidates its key immediately; there is no rotate-in-place — the documented rotation is create a new endpoint, update the sender, disable the old one.'
  in: header
  name: PloyWebhookEndpointKey
  parameter: Authorization
  scheme: bearer
  scope: single webhook endpoint
  source: https://docs.ploy.ai/webhooks
  type: http
- description: Interactive `ploy login` stores a server-side-revocable CLI refresh credential in ~/.config/ploy/config.json (mode 0600). `ploy tokens` lists up to 100 active CLI credentials; `ploy token revoke <id|name|current>` revokes one. Superseded by PLOY_API_TOKEN when that variable is set.
  in: config
  name: PloyCliBrowserLogin
  parameter: ~/.config/ploy/config.json
  scheme: bearer
  source: https://docs.ploy.ai/cli/authentication
  type: http
slug: ploy-authentication
source_filename: ploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.ploy.ai/cli/authentication\ndocs:\n- https://docs.ploy.ai/cli/authentication\n- https://docs.ploy.ai/cli/remote-development\n- https://docs.ploy.ai/webhooks\n- https://docs.ploy.ai/enhanced-security\nnote: >-\n  Ploy publishes no OpenAPI, so this profile is read from the documentation\n  rather than derived from securitySchemes. Two distinct credentials exist and\n  they are not interchangeable: a workspace-scoped API token used by the Ploy CLI\n  (and anything driving it), and a per-endpoint webhook ingest key. Both are sent\n  as HTTP bearer tokens.\nsummary:\n  types: [http]\n  schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2_note: >-\n    OAuth 2.0 appears only OUTBOUND — Ploy connects to third-party services\n    (Google, GitHub, HubSpot, Notion, Slack, Figma, ad platforms) over OAuth with\n    scoped permissions. Ploy does not publish an OAuth authorization server of\n    its own; /.well-known/oauth-authorization-server\
  \ and\n    /.well-known/openid-configuration return 404 on ploy.ai (probed 2026-08-12).\nschemes:\n- name: PloyApiToken\n  type: http\n  scheme: bearer\n  in: env\n  parameter: PLOY_API_TOKEN\n  token_prefix: sk_ploy_pat_\n  scope: workspace\n  description: >-\n    Workspace-scoped personal access token created in workspace Settings →\n    Developer → API tokens. Read by the CLI on every invocation and never written\n    to disk. Each token is pinned to exactly one workspace; the pin is enforced\n    by the API, not by the client, and a mismatched --workspace/PLOY_WORKSPACE_ID\n    exits 1 with \"This API token is scoped to a different workspace\".\n  expiry:\n    options_days: [30, 90, 365]\n    default_days: 90\n    refresh: false\n    check: ploy whoami reports the pinned workspace and remaining days\n  issuance: >-\n    The raw token is shown once, with a copyable `export PLOY_API_TOKEN=…` line.\n    It cannot be retrieved later. Any workspace member can create and view their\n   \
  \ own tokens; owners and admins can view and revoke every token in the\n    workspace.\n  restrictions: >-\n    ploy logout, ploy tokens and ploy token revoke are unavailable while\n    PLOY_API_TOKEN is set (exit code 2). API tokens cannot mint replacement\n    credentials or revoke the browser session that created them.\n  failure_modes:\n  - exit 3 — \"PLOY_API_TOKEN is invalid or expired\"\n  - exit 3 — \"PLOY_API_TOKEN is not workspace-scoped\"\n  rate_limit: 60 requests per minute per token\n  source: https://docs.ploy.ai/cli/authentication\n- name: PloyWebhookEndpointKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  scope: single webhook endpoint\n  description: >-\n    API key minted per webhook ingest endpoint in workspace Settings → Webhooks\n    and shown once. Sent as `Authorization: Bearer {apiKey}` on every POST to\n    https://ploy.ai/api/v1/webhook/{endpointSlug}. Requests without a valid key\n    are rejected with 401. Disabling or rotating\
  \ an endpoint invalidates its key\n    immediately; there is no rotate-in-place — the documented rotation is create\n    a new endpoint, update the sender, disable the old one.\n  source: https://docs.ploy.ai/webhooks\n- name: PloyCliBrowserLogin\n  type: http\n  scheme: bearer\n  in: config\n  parameter: ~/.config/ploy/config.json\n  description: >-\n    Interactive `ploy login` stores a server-side-revocable CLI refresh\n    credential in ~/.config/ploy/config.json (mode 0600). `ploy tokens` lists up\n    to 100 active CLI credentials; `ploy token revoke <id|name|current>` revokes\n    one. Superseded by PLOY_API_TOKEN when that variable is set.\n  source: https://docs.ploy.ai/cli/authentication\naccount_security:\n  passkeys: true\n  sso_saml: announced (listed as \"Coming soon\" on the Enterprise plan)\n  source: https://docs.ploy.ai/enhanced-security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploy/refs/heads/main/authentication/ploy-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Marketing
- Marketing Automation
- Artificial Intelligence
- AI Agents
- SEO
- Website Builder
- Growth
- Advertising
- Webhook
- CLI
- Agent Skills
---
