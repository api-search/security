---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Datorama Authentication
name_suffix: Authentication
oauth_flows:
- client-credentials-service-account
overview: Datorama secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client-credentials-service-account flow(s).
provider_name: Datorama
provider_slug: datorama
scheme_count: 3
schemes:
- applies_to:
  - Intelligence Platform API
  - Intelligence Query API
  - Reporting API
  bearer_prefix: false
  format: A UUID-shaped personal access token. The migration guide shows a `dato-api-` prefixed form (`dato-api-XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX`); the current platform/query docs show the bare UUID form.
  generation: Generated inside the Intelligence platform under "My Profile" (top-right menu > your name, or Ctrl+K / Cmd+K then "My Profile"). Also surfaced at the top right of the developer portal under the profile initials.
  guidance_verbatim: '"Keep your access tokens private. Access tokens should never be exposed in untrusted contexts. Never put an access token in client-side Javascript, or send it by email, instant messaging apps etc."'
  in: header
  name: IntelligenceApiToken
  parameter_name: Authorization
  rotation: Reset from the "My Profile" page.
  source: https://developers.datorama.com/docs/manage/introduction/
  type: apiKey
- applies_to:
  - MCI MCP server
  description: 'The @datorama/mci-mcp-sdk MCP server mints and refreshes a short-lived bearer from a service-account artifact JSON containing serviceAccountId, discoveryEndpoint and privateKey. The token URL is derived from the key file; there is no separately configured IdP URL. The bearer is injected into every proxied MCP message as `Authorization: Bearer ...`.'
  flow: service-account (private-key assertion against an IdP discovered from the key file)
  name: MciServiceAccountOAuth2
  source: https://www.npmjs.com/package/@datorama/mci-mcp-sdk
  token_storage: Short-lived bearer only, written atomically at mode 0600 in a 0700 state dir. The private key is held in memory only — never logged, never on argv, never persisted.
  type: oauth2
- applies_to:
  - Marketplace app -> third-party server calls
  bearer_format: JWT
  description: 'A Marketplace app calls `POST /v1/signatures` to have Intelligence issue a signed JWT, sends it to its own third-party backend as `Authorization: Bearer <jwt>`, and that backend calls `POST https://api.datorama.com/v1/signatures/verify` to confirm the request really originated from Intelligence. A verified response returns globalId, appInstanceId, env and userId — the tuple that uniquely identifies app + installation + user + environment. Unverified returns HTTP 403 and the third-party server must halt.'
  name: AppSignatureJWT
  scheme: bearer
  source: https://developers.datorama.com/docs/build/apps/making-api-calls/
  type: http
slug: datorama-authentication
source_filename: datorama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.datorama.com/docs/manage/introduction/\ndocs:\n- https://developers.datorama.com/docs/manage/introduction/\n- https://developers.datorama.com/docs/query/introduction/\n- https://developers.datorama.com/docs/query/migration-guide/\n- https://help.salesforce.com/s/articleView?id=sf.dato_getstarted_token_api.htm&type=5\nnote: >-\n  Derived from the provider's own documentation, not from a spec — Datorama publishes no OpenAPI,\n  so there are no securitySchemes to aggregate. The Platform API and the Query API share one auth\n  model: a personal API access token sent in a bare `Authorization` header (no `Bearer` prefix in\n  the documented example). The newer MCI MCP server uses a different, stronger model — OAuth2\n  service-account key exchange — which is recorded separately below.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [client-credentials-service-account]\n  token_scoping:\
  \ per-user (rate limits and permissions are enforced at the user level)\n  gated: true\n  gate_note: >-\n    API access is a PAID feature that depends on the account's plan and requires user-level\n    activation by the account manager / client success manager. A user without API access sees no\n    access token on their profile page.\nschemes:\n- name: IntelligenceApiToken\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: >-\n    A UUID-shaped personal access token. The migration guide shows a `dato-api-` prefixed form\n    (`dato-api-XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX`); the current platform/query docs show the\n    bare UUID form.\n  bearer_prefix: false\n  applies_to: [Intelligence Platform API, Intelligence Query API, Reporting API]\n  generation: >-\n    Generated inside the Intelligence platform under \"My Profile\" (top-right menu > your name, or\n    Ctrl+K / Cmd+K then \"My Profile\"). Also surfaced at the top right of the developer portal under\n  \
  \  the profile initials.\n  rotation: Reset from the \"My Profile\" page.\n  guidance_verbatim: >-\n    \"Keep your access tokens private. Access tokens should never be exposed in untrusted contexts.\n    Never put an access token in client-side Javascript, or send it by email, instant messaging\n    apps etc.\"\n  source: https://developers.datorama.com/docs/manage/introduction/\n- name: MciServiceAccountOAuth2\n  type: oauth2\n  flow: service-account (private-key assertion against an IdP discovered from the key file)\n  applies_to: [MCI MCP server]\n  description: >-\n    The @datorama/mci-mcp-sdk MCP server mints and refreshes a short-lived bearer from a\n    service-account artifact JSON containing serviceAccountId, discoveryEndpoint and privateKey.\n    The token URL is derived from the key file; there is no separately configured IdP URL. The\n    bearer is injected into every proxied MCP message as `Authorization: Bearer ...`.\n  token_storage: >-\n    Short-lived bearer only, written\
  \ atomically at mode 0600 in a 0700 state dir. The private key\n    is held in memory only — never logged, never on argv, never persisted.\n  source: https://www.npmjs.com/package/@datorama/mci-mcp-sdk\n- name: AppSignatureJWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  applies_to: [Marketplace app -> third-party server calls]\n  description: >-\n    A Marketplace app calls `POST /v1/signatures` to have Intelligence issue a signed JWT, sends it\n    to its own third-party backend as `Authorization: Bearer <jwt>`, and that backend calls\n    `POST https://api.datorama.com/v1/signatures/verify` to confirm the request really originated\n    from Intelligence. A verified response returns globalId, appInstanceId, env and userId — the\n    tuple that uniquely identifies app + installation + user + environment. Unverified returns HTTP\n    403 and the third-party server must halt.\n  source: https://developers.datorama.com/docs/build/apps/making-api-calls/\nconnector_authentication:\n\
  \  note: >-\n    Separate from API consumer auth — this is how a CUSTOM CONNECTOR authenticates to the data\n    source it pulls from. Exactly one method must be implemented per connector.\n  methods:\n  - id: user-password\n    description: >-\n      Intelligence POSTs {\"username\",\"password\"} as application/json to the connector's configured\n      loginUrl; the connector returns {\"success\": bool, \"token\": string} and the token is put on\n      the headers of every subsequent data request in that data-stream run.\n    config_shape: '{\"userPassDetails\": {\"loginUrl\": String}}'\n  source: https://developers.datorama.com/docs/build/connectors/authentication/\npermissions:\n  model: role-based, enforced server-side on the token's user\n  description: >-\n    Platform and Query endpoints serve all user roles; responses are FILTERED by role. For lower\n    roles (viewer, analyst, editor) some attributes are omitted or returned as null. Endpoints\n    restricted to specific roles\
  \ say so in their own documentation.\n  roles_reference: https://help.salesforce.com/s/articleView?id=sf.dato_getstarted_roles.htm&type=5\n  app_note: >-\n    Apps are typically installed by an Admin and then shared with non-admin users; calls that\n    require admin rights should be made during the INSTALL phase and their results persisted with\n    saveConfig.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datorama/refs/heads/main/authentication/datorama-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Analytics
- Marketing
- Marketing Intelligence
- Advertising
- Data
- Business Intelligence
- Reporting
- Salesforce
- Marketing Analytics
- Data Harmonization
- Dashboards
- MCP
---
