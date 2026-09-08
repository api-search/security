---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Adaptive''s programmatic surface authenticates with a Client App credential pair, not a single bearer token: BOTH an X-Client-ID header carrying the app''s public identifier AND an Authorization Bearer header carrying the client secret must be present. The secret is shown exactly once at creation and cannot be retrieved again. A separate, per-user OAuth 2.0 flow with RFC 7591 dynamic client registration exists for interactive MCP clients. End-user access to the platform itself is a third, distinct path (SSO/MFA via Okta, Azure AD, Google, JumpCloud, OneLogin or LDAP) and is not an API credential.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Adaptive Automation Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adaptive Automation Technologies declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Adaptive Automation Technologies
provider_slug: adaptive-automation-technologies
scheme_count: 4
schemes:
- applies_to: All sixteen REST Client API operations and the headless MCP endpoint.
  docs: https://documentation.adaptive.live/developer-guide/adaptive-api
  failure_modes:
  - body: '{"error":"bad service token: empty service token"}'
    status: 401
    when: No or malformed credential. Observed live on 2026-09-07.
  - body: operation not permitted for this key
    status: 403
    when: The key is restricted and lacks a scope the endpoint requires.
  id: client_app
  provisioning: Organization > Client Apps > Add Client > Generate Client Secret. The secret is displayed once and never shown again.
  required_headers:
  - in: header
    name: X-Client-ID
    required: true
    value: The Client App's public identifier
  - in: header
    name: Authorization
    required: true
    value: Bearer <client-secret>
  - in: header
    name: Content-Type
    required: true
    value: application/json
  revocation: Deleting a Client App immediately stops both its API requests and any MCP connections that use it.
  scope_model: Full access (default, and the behaviour of every key created before scopes existed) or Restricted to a selected subset of the ten operation scopes. Scopes are fixed at creation — to change them you delete the key and create a new one.
  scoped: true
  scopes_detail: scopes/adaptive-automation-technologies-scopes.yml
  type: composite
- applies_to: Interactive MCP clients connecting to https://<workspace-url>/mcp
  dcr_spec: RFC 7591
  docs: https://documentation.adaptive.live/platform/organization/mcp-servers
  dynamic_client_registration: true
  endpoints_note: Issuer, Authorization, Token and Registration endpoint URLs are exposed inside the authenticated Organization > MCP Servers tab. Probes of /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource on every host returned 404 (or an SPA soft-404 on app.adaptive.live), so a client cannot discover them anonymously — see well-known/.
  endpoints_published_at_well_known: false
  flow: authorization_code (browser consent screen)
  id: mcp_oauth
  optional_binding: A token may be bound to an existing Client App, intersecting its scopes with that app's allowed operations.
  revocation: Per-token revoke, and per-client delete, from the MCP Servers tab.
  scope_ceiling: The scope list offered at consent is always capped at the connecting user's own role, so an agent can never do more than the person who authorized it.
  token_lifetime_options:
  - 1 day
  - 30 days
  - 90 days
  - 1 year
  - until revoked
  type: oauth2
- applies_to: The Terraform and Pulumi providers
  detail: 'A service account token generated in the Adaptive console. Terraform reads it from the `service_token` provider argument, falling back to the adaptive-cli token. Pulumi reads it from `adaptive:serviceToken` stack config, then the ADAPTIVE_SVC_TOKEN environment variable, then ~/.adaptive/token written by `adaptive login`. Where that file lists multiple deployments, exactly one must be marked "default": true — the provider refuses an ambiguous file rather than picking one at random.'
  docs: https://documentation.adaptive.live/developer-guide/terraform
  id: service_token
  type: apiKey
- applies_to: The Adaptive CLI
  detail: '`adaptive login` opens a browser authentication prompt and writes a token to ~/.adaptive/token. Multiple named contexts/profiles are supported (`adaptive login --context-name staging --url https://staging.url.com`).'
  docs: https://documentation.adaptive.live/developer-guide/adaptive-cli
  id: cli_login
  type: browser
slug: adaptive-automation-technologies-authentication
source_filename: adaptive-automation-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://documentation.adaptive.live/developer-guide/adaptive-api and\n  https://documentation.adaptive.live/platform/organization/mcp-servers. Derived from\n  documentation rather than from a spec — Adaptive publishes no OpenAPI, so there are no\n  securitySchemes to read.\ndescription: >-\n  Adaptive's programmatic surface authenticates with a Client App credential pair, not a\n  single bearer token: BOTH an X-Client-ID header carrying the app's public identifier AND\n  an Authorization Bearer header carrying the client secret must be present. The secret is\n  shown exactly once at creation and cannot be retrieved again. A separate, per-user OAuth\n  2.0 flow with RFC 7591 dynamic client registration exists for interactive MCP clients.\n  End-user access to the platform itself is a third, distinct path (SSO/MFA via Okta, Azure\n  AD, Google, JumpCloud, OneLogin or LDAP) and is not an API credential.\nbase_url: https://app.adaptive.live\n\
  base_url_note: >-\n  Managed cloud. Self-hosted deployments substitute their own workspace host; the docs write\n  the base as https://<your-domain>.adaptive.live and the Pulumi provider defaults\n  workspaceUrl to https://app.adaptive.live.\nschemes:\n- id: client_app\n  type: composite\n  applies_to: All sixteen REST Client API operations and the headless MCP endpoint.\n  required_headers:\n  - name: X-Client-ID\n    in: header\n    value: The Client App's public identifier\n    required: true\n  - name: Authorization\n    in: header\n    value: Bearer <client-secret>\n    required: true\n  - name: Content-Type\n    in: header\n    value: application/json\n    required: true\n  provisioning: >-\n    Organization > Client Apps > Add Client > Generate Client Secret. The secret is displayed\n    once and never shown again.\n  revocation: >-\n    Deleting a Client App immediately stops both its API requests and any MCP connections\n    that use it.\n  scoped: true\n  scopes_detail: scopes/adaptive-automation-technologies-scopes.yml\n\
  \  scope_model: >-\n    Full access (default, and the behaviour of every key created before scopes existed) or\n    Restricted to a selected subset of the ten operation scopes. Scopes are fixed at\n    creation — to change them you delete the key and create a new one.\n  failure_modes:\n  - status: 401\n    body: '{\"error\":\"bad service token: empty service token\"}'\n    when: No or malformed credential. Observed live on 2026-09-07.\n  - status: 403\n    body: operation not permitted for this key\n    when: The key is restricted and lacks a scope the endpoint requires.\n  docs: https://documentation.adaptive.live/developer-guide/adaptive-api\n- id: mcp_oauth\n  type: oauth2\n  applies_to: Interactive MCP clients connecting to https://<workspace-url>/mcp\n  flow: authorization_code (browser consent screen)\n  dynamic_client_registration: true\n  dcr_spec: RFC 7591\n  endpoints_published_at_well_known: false\n  endpoints_note: >-\n    Issuer, Authorization, Token and Registration endpoint\
  \ URLs are exposed inside the\n    authenticated Organization > MCP Servers tab. Probes of\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource on\n    every host returned 404 (or an SPA soft-404 on app.adaptive.live), so a client cannot\n    discover them anonymously — see well-known/.\n  token_lifetime_options: [1 day, 30 days, 90 days, 1 year, until revoked]\n  scope_ceiling: >-\n    The scope list offered at consent is always capped at the connecting user's own role, so\n    an agent can never do more than the person who authorized it.\n  optional_binding: >-\n    A token may be bound to an existing Client App, intersecting its scopes with that app's\n    allowed operations.\n  revocation: Per-token revoke, and per-client delete, from the MCP Servers tab.\n  docs: https://documentation.adaptive.live/platform/organization/mcp-servers\n- id: service_token\n  type: apiKey\n  applies_to: The Terraform and Pulumi providers\n  detail: >-\n    A service account\
  \ token generated in the Adaptive console. Terraform reads it from the\n    `service_token` provider argument, falling back to the adaptive-cli token. Pulumi reads\n    it from `adaptive:serviceToken` stack config, then the ADAPTIVE_SVC_TOKEN environment\n    variable, then ~/.adaptive/token written by `adaptive login`. Where that file lists\n    multiple deployments, exactly one must be marked \"default\": true — the provider refuses\n    an ambiguous file rather than picking one at random.\n  docs: https://documentation.adaptive.live/developer-guide/terraform\n- id: cli_login\n  type: browser\n  applies_to: The Adaptive CLI\n  detail: >-\n    `adaptive login` opens a browser authentication prompt and writes a token to\n    ~/.adaptive/token. Multiple named contexts/profiles are supported\n    (`adaptive login --context-name staging --url https://staging.url.com`).\n  docs: https://documentation.adaptive.live/developer-guide/adaptive-cli\nplatform_identity:\n  note: >-\n    Human sign-in\
  \ to the platform is separate from API credentials and is federated.\n  providers: [Okta, Azure Active Directory, Google SSO, JumpCloud, OneLogin, LDAP]\n  mfa: Enforced on resources per Adaptive's access policy.\n  docs: https://documentation.adaptive.live/integrations/all\nx-evidence:\n- url: https://app.adaptive.live/api/v3/client/users/list\n  http_status: 401\n  body: '{\"error\":\"bad service token: empty service token\"}'\n  fetched: '2026-09-07'\n- url: https://documentation.adaptive.live/developer-guide/adaptive-api\n  http_status: 200\n  fetched: '2026-09-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-automation-technologies/refs/heads/main/authentication/adaptive-automation-technologies-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Data Security
- Agents
- Model Context Protocol
- Infrastructure
- Databases
- Kubernetes
- Compliance
- Audit
---
