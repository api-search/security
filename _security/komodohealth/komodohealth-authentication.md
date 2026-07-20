---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Komodohealth Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
- clientCredentials
overview: Komodo Health secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode and clientCredentials flow(s).
provider_name: Komodo Health
provider_slug: komodohealth
scheme_count: 2
schemes:
- credential: JWT bearer token
  description: Browser-based OAuth 2.0 Device Authorization Flow for interactive users. Started with `komodo login`; stores a JWT plus refresh token. Triggered automatically by the SDK when no credentials are found (in that case the credentials live in memory only and are not persisted).
  flow: deviceCode
  name: WebLogin
  persisted_to: ~/.komodo/credentials
  profile: '[default]'
  requires:
  - account_id
  sources:
  - docs
  type: oauth2
- credential: client_id + client_secret
  description: Machine-to-machine authentication using service-principal credentials for automation, CI/CD, and services. No user interaction required.
  flow: clientCredentials
  name: ServicePrincipal
  persisted_to: ~/.komodo/credentials
  profile: named profile (e.g. [production], [development])
  provisioning: uv run komodo service-principal create --name "my-service"
  requires:
  - account_id
  sources:
  - docs
  type: oauth2
slug: komodohealth-authentication
source_filename: komodohealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.komodohealth.com/guides-tutorials/guides/2-authentication/\ndocs: https://docs.komodohealth.com/guides-tutorials/guides/2-authentication/\nnotes: >-\n  Derived by SEARCH of the published authentication guide and SDK/CLI reference.\n  Komodo Health publishes no public OpenAPI document\n  (https://api.komodohealth.com/openapi.json returns 401), so the scheme set\n  below is captured from documentation rather than from securitySchemes.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [deviceCode, clientCredentials]\n  token_format: JWT\n  account_scoped: true\n  api_key_in: []\nschemes:\n- name: WebLogin\n  type: oauth2\n  flow: deviceCode\n  description: >-\n    Browser-based OAuth 2.0 Device Authorization Flow for interactive users.\n    Started with `komodo login`; stores a JWT plus refresh token. Triggered\n    automatically by the SDK when no credentials are found (in that case the\n    credentials live in memory\
  \ only and are not persisted).\n  credential: JWT bearer token\n  persisted_to: ~/.komodo/credentials\n  profile: '[default]'\n  requires: [account_id]\n  sources: [docs]\n- name: ServicePrincipal\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Machine-to-machine authentication using service-principal credentials for\n    automation, CI/CD, and services. No user interaction required.\n  credential: client_id + client_secret\n  provisioning: uv run komodo service-principal create --name \"my-service\"\n  persisted_to: ~/.komodo/credentials\n  profile: named profile (e.g. [production], [development])\n  requires: [account_id]\n  sources: [docs]\nscopes:\n  documented: false\n  note: >-\n    Komodo publishes no OAuth scope/permission reference. Authorization is\n    account-scoped (each account has an isolated, Komodo-managed Snowflake\n    warehouse) with Snowflake roles applied inside it, plus RBAC/FGA app roles\n    for the App Builder surface. No scopes/ artifact is\
  \ emitted.\naccounts:\n  model: >-\n    A Komodo account is the organizational entity on the platform. Each account\n    has its own data subscriptions and a dedicated Komodo-managed Snowflake\n    warehouse. Every query and API operation is scoped to the selected account.\n    Accounts are isolated — data does not move between them.\n  identifiers:\n  - {name: account_id, format: UUID, example_shape: 8-4-4-4-12}\n  - {name: account_slug, format: human-readable string}\n  selection: uv run komodo account set\ncredentials_file:\n  default_path: ~/.komodo/credentials\n  format: INI-style named profiles\n  override_env: KOMODO_CREDENTIALS_PATH\n  tilde_expansion: true\n  fields_default_profile: [token, token_expiration, account_id, account_slug]\n  fields_m2m_profile: [client_id, client_secret, account_id, account_slug]\nprecedence:\n- rank: 1\n  description: Explicit credentials passed to the SDK function (jwt + account_id, client_id + client_secret + account_id, or profile)\n- rank: 2\n\
  \  description: '[default] profile from ~/.komodo/credentials (written by `komodo login`)'\n- rank: 3\n  description: Browser web-login flow triggered by the SDK (not persisted to disk)\nconstraints:\n- Only one authentication method may be used at a time.\n- JWT and explicit M2M credentials both require an account_id.\n- A profile cannot be combined with account_id — the profile already contains it.\n- jwt cannot be mixed with client_id / client_secret.\n- Named profiles support M2M credentials only, not JWT tokens.\ntoken_refresh:\n  automatic: true\n  note: The SDK refreshes JWTs automatically via the stored refresh token.\nrelated:\n  conventions: conventions/komodohealth-conventions.yml\n  errors: errors/komodohealth-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komodohealth/refs/heads/main/authentication/komodohealth-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Data
- Life Sciences
- Real-World Data
- Real-World Evidence
- Healthcare AI
- Analytics
- Data Platform
- Snowflake
- Python SDK
- MCP
---
