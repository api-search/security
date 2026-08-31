---
api_key_in: []
api_specs:
- filename: leanlaw-client-api-openapi.yml
  format: yaml
  label: LeanLaw Client API
  slug: leanlaw-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-client-api-openapi.yml
- filename: leanlaw-codes-api-openapi.yml
  format: yaml
  label: LeanLaw Codes API
  slug: leanlaw-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-codes-api-openapi.yml
- filename: leanlaw-customfield-api-openapi.yml
  format: yaml
  label: LeanLaw Custom Field API
  slug: leanlaw-customfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-customfield-api-openapi.yml
- filename: leanlaw-expense-api-openapi.yml
  format: yaml
  label: LeanLaw Expense API
  slug: leanlaw-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-expense-api-openapi.yml
- filename: leanlaw-fixedfee-api-openapi.yml
  format: yaml
  label: LeanLaw Fixed Fee API
  slug: leanlaw-fixedfee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-fixedfee-api-openapi.yml
- filename: leanlaw-invoice-api-openapi.yml
  format: yaml
  label: LeanLaw Invoice API
  slug: leanlaw-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-invoice-api-openapi.yml
- filename: leanlaw-matter-api-openapi.yml
  format: yaml
  label: LeanLaw Matter API
  slug: leanlaw-matter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-matter-api-openapi.yml
- filename: leanlaw-practicearea-api-openapi.yml
  format: yaml
  label: LeanLaw Practice Area API
  slug: leanlaw-practicearea-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-practicearea-api-openapi.yml
- filename: leanlaw-timeentry-api-openapi.yml
  format: yaml
  label: LeanLaw Time Entry API
  slug: leanlaw-timeentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-timeentry-api-openapi.yml
- filename: leanlaw-user-api-openapi.yml
  format: yaml
  label: LeanLaw User API
  slug: leanlaw-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Leanlaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeanLaw secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeanLaw
provider_slug: leanlaw
scheme_count: 2
schemes:
- applied: global
  description: A LeanLaw API key presented as a bearer token. The key represents the ACCOUNT (the firm), not an individual user, and acts on behalf of the firm with the scopes selected when the key was created.
  format: 'Authorization: Bearer {apikey}'
  header: Authorization
  in: header
  name: BearerAuth
  operations_covered: 35
  provisioning:
    action: Generate API Key
    display: shown once at creation; must be stored by the caller
    requires: firm setup / administrator access
    scope_selection: read or write permissions chosen per key at creation time
    ui_path: Settings > API
  scheme: bearer
  sources:
  - openapi/leanlaw-api-openapi.json
  - https://platform.leanlaw.io/auth
  transport: HTTPS required
  type: http
- applied: MCP / agent surface only
  description: OAuth 2.1 authorization-code + PKCE against https://auth.myleanlaw.co/, used to authorize AI assistants against the MCP server. Unlike the firm-wide API key this is per USER — the connection carries only that person's access. Documented as private beta.
  flows:
    authorizationCode:
      authorizationUrl: https://api.myleanlaw.co/oauth/authorize
      refreshUrl: https://api.myleanlaw.co/oauth/token
      revocationUrl: https://api.myleanlaw.co/oauth/revoke
      tokenUrl: https://api.myleanlaw.co/oauth/token
  in_openapi: false
  name: OAuth2
  scopes: scopes/leanlaw-scopes.yml
  sources:
  - https://api.leanlaw.io/.well-known/oauth-protected-resource
  - https://api.myleanlaw.co/.well-known/openid-configuration
  - https://platform.leanlaw.io/agents
  type: oauth2
slug: leanlaw-authentication
source_filename: leanlaw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://platform.leanlaw.io/auth\ndocs: https://platform.leanlaw.io/auth\nalso_derived_from: openapi/leanlaw-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: API key presented as an HTTP bearer token\n  note: >-\n    The published OpenAPI declares exactly one scheme (BearerAuth, http/bearer) applied globally to\n    all 35 operations. The docs additionally document two request headers that are NOT in the spec\n    (x-leanlaw-userid, x-leanlaw-partnerid), and a separate OAuth 2.1 authorization server used for\n    the MCP/agent surface that is likewise absent from the spec.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {apikey}'\n  applied: global\n  operations_covered: 35\n  sources:\n  - openapi/leanlaw-api-openapi.json\n  - https://platform.leanlaw.io/auth\n  description: >-\n    A LeanLaw API key presented as a\
  \ bearer token. The key represents the ACCOUNT (the firm), not an\n    individual user, and acts on behalf of the firm with the scopes selected when the key was created.\n  provisioning:\n    ui_path: Settings > API\n    action: Generate API Key\n    scope_selection: read or write permissions chosen per key at creation time\n    display: shown once at creation; must be stored by the caller\n    requires: firm setup / administrator access\n  transport: HTTPS required\n- name: OAuth2\n  type: oauth2\n  applied: MCP / agent surface only\n  in_openapi: false\n  sources:\n  - https://api.leanlaw.io/.well-known/oauth-protected-resource\n  - https://api.myleanlaw.co/.well-known/openid-configuration\n  - https://platform.leanlaw.io/agents\n  description: >-\n    OAuth 2.1 authorization-code + PKCE against https://auth.myleanlaw.co/, used to authorize AI\n    assistants against the MCP server. Unlike the firm-wide API key this is per USER — the connection\n    carries only that person's access.\
  \ Documented as private beta.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.myleanlaw.co/oauth/authorize\n      tokenUrl: https://api.myleanlaw.co/oauth/token\n      refreshUrl: https://api.myleanlaw.co/oauth/token\n      revocationUrl: https://api.myleanlaw.co/oauth/revoke\n  scopes: scopes/leanlaw-scopes.yml\nsupplemental_headers:\n- name: x-leanlaw-userid\n  required: false\n  in_openapi: false\n  description: >-\n    Identifies the acting user for calls that otherwise operate at firm scope. Documented as the\n    recommended approach for time-tracking use cases so matter and time-entry lists are scoped to one\n    user. The userId comes from the ListUsers endpoint.\n  source: https://platform.leanlaw.io/auth\n- name: x-leanlaw-partnerid\n  required: false\n  in_openapi: false\n  description: LeanLaw partners must send their partner id on all requests.\n  source: https://platform.leanlaw.io/auth\ngaps:\n- The API key is firm-scoped rather than user-scoped, so\
  \ per-user attribution depends on the caller\n  voluntarily sending x-leanlaw-userid.\n- Neither x-leanlaw-userid nor x-leanlaw-partnerid appears in the OpenAPI, so a generated client will\n  not expose them.\n- The OAuth 2.1 surface is fully discoverable at runtime but is not represented in the OpenAPI\n  securitySchemes, so spec-driven tooling sees only the bearer API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/authentication/leanlaw-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Legal
- Legal Billing
- Law Firms
- Time Tracking
- Billing
- Invoicing
- Accounting
- Trust Accounting
- Practice Management
- QuickBooks
- Payments
- LegalTech
- SaaS
---
