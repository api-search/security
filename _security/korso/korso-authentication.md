---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Korso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Korso secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Korso
provider_slug: korso
scheme_count: 3
schemes:
- deployment: korso-hosted
  description: Account-scoped token that works across every workspace the account belongs to - there is no per-repo or per-workspace re-tokening. Wins if TEAM_TOKEN is also set.
  issued_via: Sign in to the Korso dashboard with Google or GitHub, open the Connect Agent panel, optionally name the token, then click Generate token.
  management: Tokens can be named, listed with created and last-used timestamps, and individually revoked from the Connect Agent panel at any time.
  name: SHEPHERD_TOKEN
  revocable: true
  scheme: bearer
  scope: account
  shown_once: true
  sources:
  - https://korsoai.com/docs/guides/authentication
  token_prefix: shp_
  type: http
- deployment: self-hosted
  description: A single shared, workspace-wide secret. Not scoped per agent or per person - anyone holding it has full authority over that hub's one workspace. Documented as a shared password, not an identity.
  issued_via: Configured on the hub by whoever operates it and distributed to the team.
  name: TEAM_TOKEN
  revocable: rotate on the hub
  scheme: bearer
  scope: workspace
  shown_once: false
  sources:
  - https://korsoai.com/docs/guides/authentication
  type: http
  warning: Never commit it; distribute through a secret manager and rotate it if a teammate with access leaves.
- deployment: korso-hosted (internal)
  description: The hosted deployment mode authenticates the front-end/BFF to the hub with an internal token plus a trusted x-account-id header, then mints per-agent tokens. Documented in the Shepherd AGENTS.md and implemented in packages/hub/src/tenant.ts. Not a public developer-facing credential.
  name: x-internal-token + x-account-id
  scheme: custom-header
  sources:
  - https://github.com/Korso-AI/Shepherd/blob/main/AGENTS.md
  type: http
slug: korso-authentication
source_filename: korso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://korsoai.com/docs/guides/authentication\ndocs: https://korsoai.com/docs/guides/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  note: >-\n    No OpenAPI is published, so this profile is captured from the provider's authentication guide rather\n    than derived from securitySchemes. Shepherd has no OAuth scope surface - both credential kinds are\n    opaque bearer tokens - so no scopes/ artifact is emitted.\nschemes:\n- name: SHEPHERD_TOKEN\n  type: http\n  scheme: bearer\n  deployment: korso-hosted\n  scope: account\n  token_prefix: shp_\n  issued_via: >-\n    Sign in to the Korso dashboard with Google or GitHub, open the Connect Agent panel, optionally name\n    the token, then click Generate token.\n  shown_once: true\n  revocable: true\n  management: >-\n    Tokens can be named, listed with created and last-used timestamps, and individually revoked\
  \ from the\n    Connect Agent panel at any time.\n  description: >-\n    Account-scoped token that works across every workspace the account belongs to - there is no per-repo\n    or per-workspace re-tokening. Wins if TEAM_TOKEN is also set.\n  sources:\n  - https://korsoai.com/docs/guides/authentication\n- name: TEAM_TOKEN\n  type: http\n  scheme: bearer\n  deployment: self-hosted\n  scope: workspace\n  issued_via: Configured on the hub by whoever operates it and distributed to the team.\n  shown_once: false\n  revocable: rotate on the hub\n  description: >-\n    A single shared, workspace-wide secret. Not scoped per agent or per person - anyone holding it has\n    full authority over that hub's one workspace. Documented as a shared password, not an identity.\n  warning: >-\n    Never commit it; distribute through a secret manager and rotate it if a teammate with access leaves.\n  sources:\n  - https://korsoai.com/docs/guides/authentication\n- name: x-internal-token + x-account-id\n  type:\
  \ http\n  scheme: custom-header\n  deployment: korso-hosted (internal)\n  description: >-\n    The hosted deployment mode authenticates the front-end/BFF to the hub with an internal token plus a\n    trusted x-account-id header, then mints per-agent tokens. Documented in the Shepherd AGENTS.md and\n    implemented in packages/hub/src/tenant.ts. Not a public developer-facing credential.\n  sources:\n  - https://github.com/Korso-AI/Shepherd/blob/main/AGENTS.md\ntransport:\n  mechanism: environment variables on the stdio MCP server process\n  required: at least one of SHEPHERD_TOKEN or TEAM_TOKEN\n  failure_mode: >-\n    The @korso/shepherd MCP server fails immediately at startup with a clear error when neither variable\n    is set.\n  companion_variables:\n  - name: HUB_URL\n    description: Base URL of the Shepherd hub.\n  - name: WORKSPACE\n    description: >-\n      Self-host only; must exactly match the hub's configured workspace. Ignored on the hosted path.\nidentity_model:\n  account:\
  \ >-\n    On a hosted hub, whatever the user signed in with (Google or GitHub). On self-host, effectively\n    whoever holds the TEAM_TOKEN.\n  workspace: A coordination boundary; every coordination table carries a NOT NULL workspace_id.\n  repo: >-\n    Opted into a workspace by a committed .shepherd marker file naming the workspace slug - never a\n    token.\n  membership: >-\n    A repo can only be linked to a workspace the account is a member of; invalid slugs are rejected.\n  token_storage: Hashed shp_ API tokens; the raw value is shown once and cannot be retrieved again.\nidentity_providers:\n- Google\n- GitHub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korso/refs/heads/main/authentication/korso-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Model Context Protocol
- Developer Tools
- Open Source
- Agent Coordination
- Y Combinator
---
