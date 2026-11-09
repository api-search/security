---
anonymous_access: false
api_key_in: []
auth_types:
- http
- oauth2
description: 'Delphina''s HTTP API and its MCP server both accept bearer credentials over HTTPS. Three credential types are documented: (1) a personal, long-lived API key issued in User Settings > API Key, (2) personal API tokens with optional expiration (7/30/90/180/365 days or no expiration) issued and revoked from User Settings > API Key, and (3) service-account tokens issued per workspace from Org Admin > Service Accounts for machine-to- machine access. The MCP server at `app.delphina.ai/api/mcp` also supports OAuth 2.0 authorization code (preferred by the docs because nothing long-lived has to be copied into client configuration); the Delphina Claude Code and Codex plugins use OAuth by default. Workspace sign-in at analytics.delphina.ai is federated through SSO (Google Workspace, Okta, Microsoft Entra ID, or any SAML/OIDC provider).'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Delphina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delphina secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Delphina
provider_slug: delphina
scheme_count: 3
schemes:
- description: '`Authorization: Bearer YOUR_TOKEN` — accepted on every HTTP API path

    under `https://app.delphina.ai/api` and on the MCP server at

    `https://app.delphina.ai/api/mcp`. The token can be a personal API

    key, a personal API token, or a service-account token; all three

    travel the same way on the wire and differ only in how they are

    issued and revoked.

    '
  docs: https://docs.delphina.ai/administration/service-accounts
  key_types:
  - expiration: none (long-lived)
    issued_at: User Settings > API Key
    name: personal-api-key
    rotatable: re-copyable from the page at any time
  - expiration_options:
    - no expiration
    - 7 days
    - 30 days
    - 90 days
    - 180 days
    - 365 days
    issued_at: User Settings > API Key > API tokens
    name: personal-api-token
    revocation: immediate per-token, cannot be undone
    shown_once: full token displayed once at creation; only prefix + last four shown after
  - expiration_options:
    - no expiration
    - 7 days
    - 30 days
    - 90 days
    - 180 days
    - 365 days
    identity_format: name@<org>.svc.delphina.ai (permanent; up to 64 chars, lowercase letters, digits, and hyphens — not at the start or end)
    issued_at: Org Admin > Service Accounts
    name: service-account-token
    revocation: immediate per-token, cannot be undone
    shown_once: true
  name: bearer
  scheme: bearer
  type: http
- description: 'OAuth 2.0 authorization code flow, used for MCP client authorization

    against `https://app.delphina.ai/api/mcp`. Supported clients

    (Claude Code, Claude Desktop/Cowork, Codex, Cursor) complete the

    browser-based sign-in; no long-lived key is stored in client

    configuration.

    '
  docs: https://docs.delphina.ai/integrations/delphina-mcp
  endpoint: https://app.delphina.ai/api/mcp
  flow: authorization_code
  name: oauth2
  note: Delphina also acts as an OAuth client to downstream MCP providers (Notion, Linear, Attio …) on the MCP Connections page; the redirect URI it requires the provider to allow is `https://app.delphina.ai/api/auth/v1/oauth2/mcp/callback`. That is an outbound OAuth role, not an inbound one.
  preferred: true
  scopes_doc: null
  type: oauth2
- description: 'End-user sign-in to the Delphina web app is federated through the

    organization''s SSO provider. Supported providers named by the docs:

    Google Workspace, Okta (SAML and OIDC), Microsoft Entra ID, and

    "other SAML/OIDC providers". No separate Delphina passwords.

    '
  docs: https://docs.delphina.ai/administration/sso
  name: sso
  providers:
  - google-workspace
  - okta
  - microsoft-entra-id
  - other-saml-oidc
  type: oidc
slug: delphina-authentication
source_filename: delphina-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.delphina.ai/administration/service-accounts.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://docs.delphina.ai/administration/service-accounts.md\nsources:\n  - https://docs.delphina.ai/administration/service-accounts.md\n  - https://docs.delphina.ai/user-settings.md\n  - https://docs.delphina.ai/integrations/delphina-mcp.md\n  - https://docs.delphina.ai/administration/sso.md\ndocs: https://docs.delphina.ai/administration/service-accounts\ndescription: >-\n  Delphina's HTTP API and its MCP server both accept bearer credentials over\n  HTTPS. Three credential types are documented: (1) a personal, long-lived\n  API key issued in User Settings > API Key, (2) personal API tokens with\n  optional expiration (7/30/90/180/365 days or no expiration) issued and\n  revoked from User Settings > API Key, and (3) service-account tokens\n  issued per workspace from Org Admin > Service Accounts for machine-to-\n  machine access. The MCP server at `app.delphina.ai/api/mcp` also\n  supports OAuth 2.0 authorization code (preferred\
  \ by the docs because\n  nothing long-lived has to be copied into client configuration); the\n  Delphina Claude Code and Codex plugins use OAuth by default. Workspace\n  sign-in at analytics.delphina.ai is federated through SSO (Google\n  Workspace, Okta, Microsoft Entra ID, or any SAML/OIDC provider).\nsummary:\n  types:\n    - http\n    - oauth2\n  key_scheme: Bearer token in the `Authorization` header\n  mfa: via upstream SSO provider\nschemes:\n  - name: bearer\n    type: http\n    scheme: bearer\n    description: |\n      `Authorization: Bearer YOUR_TOKEN` — accepted on every HTTP API path\n      under `https://app.delphina.ai/api` and on the MCP server at\n      `https://app.delphina.ai/api/mcp`. The token can be a personal API\n      key, a personal API token, or a service-account token; all three\n      travel the same way on the wire and differ only in how they are\n      issued and revoked.\n    key_types:\n      - name: personal-api-key\n        issued_at: User Settings > API\
  \ Key\n        rotatable: re-copyable from the page at any time\n        expiration: none (long-lived)\n      - name: personal-api-token\n        issued_at: User Settings > API Key > API tokens\n        expiration_options: [no expiration, 7 days, 30 days, 90 days, 180 days, 365 days]\n        revocation: immediate per-token, cannot be undone\n        shown_once: full token displayed once at creation; only prefix + last four shown after\n      - name: service-account-token\n        issued_at: Org Admin > Service Accounts\n        expiration_options: [no expiration, 7 days, 30 days, 90 days, 180 days, 365 days]\n        revocation: immediate per-token, cannot be undone\n        shown_once: true\n        identity_format: 'name@<org>.svc.delphina.ai (permanent; up to 64 chars, lowercase letters, digits, and hyphens — not at the start or end)'\n    docs: https://docs.delphina.ai/administration/service-accounts\n  - name: oauth2\n    type: oauth2\n    description: |\n      OAuth 2.0 authorization\
  \ code flow, used for MCP client authorization\n      against `https://app.delphina.ai/api/mcp`. Supported clients\n      (Claude Code, Claude Desktop/Cowork, Codex, Cursor) complete the\n      browser-based sign-in; no long-lived key is stored in client\n      configuration.\n    flow: authorization_code\n    endpoint: https://app.delphina.ai/api/mcp\n    preferred: true\n    docs: https://docs.delphina.ai/integrations/delphina-mcp\n    scopes_doc: null\n    note: >-\n      Delphina also acts as an OAuth client to downstream MCP providers\n      (Notion, Linear, Attio …) on the MCP Connections page; the redirect\n      URI it requires the provider to allow is\n      `https://app.delphina.ai/api/auth/v1/oauth2/mcp/callback`. That is\n      an outbound OAuth role, not an inbound one.\n  - name: sso\n    type: oidc\n    description: |\n      End-user sign-in to the Delphina web app is federated through the\n      organization's SSO provider. Supported providers named by the docs:\n     \
  \ Google Workspace, Okta (SAML and OIDC), Microsoft Entra ID, and\n      \"other SAML/OIDC providers\". No separate Delphina passwords.\n    providers: [google-workspace, okta, microsoft-entra-id, other-saml-oidc]\n    docs: https://docs.delphina.ai/administration/sso\nunauthenticated_response:\n  status: 401\n  body: '\"No authentication!\"'\n  note: Observed by the identity probe on paths under https://app.delphina.ai/api; recorded in apis.yml.\n"
source_yaml_url: https://artifacts.apis.io/delphina/authentication/delphina-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Technology
- Data
- Platform
---
