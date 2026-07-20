---
api_key_in: []
auth_types: []
description: 'How callers authenticate to the Komodo Health platform. Komodo supports two mutually exclusive modes: interactive web login (OAuth 2.0 Device Authorization Flow, yielding a JWT) and machine-to-machine service-principal credentials (client_id / client_secret). Every call is scoped to a Komodo account, each of which maps to a dedicated Komodo-managed Snowflake warehouse. Derived from the published auth guide — Komodo does not publish an OpenAPI document, so these schemes are documented rather than machine-read.'
kind: authentication
layout: security
method: searched
name: Komodo Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Komodo Health declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Komodo Health
provider_slug: komodo-health
scheme_count: 3
schemes:
- description: Browser-based OAuth flow for interactive users. Started with `komodo login`; opens the browser, then persists the JWT and refresh token to the [default] profile in ~/.komodo/credentials. Intended for individual, manual use.
  flow: device_authorization
  id: web_login
  note: If no credentials are found the SDK triggers a web login automatically, but those credentials are in-memory only and are not written to disk.
  persisted: true
  persisted_to: ~/.komodo/credentials
  rfc: RFC 8628
  token_command: komodo jwt
  token_type: JWT
  type: oauth2
- credentials:
  - client_id
  - client_secret
  description: Machine-to-machine authentication for automation, CI/CD and services. Service principals are created with `komodo service-principal create`, which returns a client_id and client_secret. No user interaction required.
  flow: client_credentials
  id: service_principal
  management_commands:
  - komodo service-principal create --name "<name>" --description "<desc>"
  - komodo service-principal list
  - komodo service-principal delete <SERVICE_PRINCIPAL_ID>
  requires: account_id (or a named profile that carries it)
  type: oauth2
- description: A JWT obtained from `komodo jwt` may be passed directly into the SDK alongside an account_id. In-memory only.
  id: explicit_jwt
  scheme: bearer
  type: http
slug: komodo-health-authentication
source_filename: komodo-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.komodohealth.com/guides-tutorials/guides/2-authentication\ndescription: >-\n  How callers authenticate to the Komodo Health platform. Komodo supports two\n  mutually exclusive modes: interactive web login (OAuth 2.0 Device\n  Authorization Flow, yielding a JWT) and machine-to-machine service-principal\n  credentials (client_id / client_secret). Every call is scoped to a Komodo\n  account, each of which maps to a dedicated Komodo-managed Snowflake warehouse.\n  Derived from the published auth guide — Komodo does not publish an OpenAPI\n  document, so these schemes are documented rather than machine-read.\ndocs: https://docs.komodohealth.com/guides-tutorials/guides/2-authentication\n\nschemes:\n  - id: web_login\n    type: oauth2\n    flow: device_authorization\n    rfc: RFC 8628\n    description: >-\n      Browser-based OAuth flow for interactive users. Started with `komodo\n      login`; opens the browser, then\
  \ persists the JWT and refresh token to the\n      [default] profile in ~/.komodo/credentials. Intended for individual,\n      manual use.\n    token_type: JWT\n    token_command: komodo jwt\n    persisted: true\n    persisted_to: ~/.komodo/credentials\n    note: >-\n      If no credentials are found the SDK triggers a web login automatically,\n      but those credentials are in-memory only and are not written to disk.\n  - id: service_principal\n    type: oauth2\n    flow: client_credentials\n    description: >-\n      Machine-to-machine authentication for automation, CI/CD and services.\n      Service principals are created with `komodo service-principal create`,\n      which returns a client_id and client_secret. No user interaction required.\n    credentials: [client_id, client_secret]\n    requires: account_id (or a named profile that carries it)\n    management_commands:\n      - komodo service-principal create --name \"<name>\" --description \"<desc>\"\n      - komodo service-principal\
  \ list\n      - komodo service-principal delete <SERVICE_PRINCIPAL_ID>\n  - id: explicit_jwt\n    type: http\n    scheme: bearer\n    description: >-\n      A JWT obtained from `komodo jwt` may be passed directly into the SDK\n      alongside an account_id. In-memory only.\n\naccount_scoping:\n  required: true\n  description: >-\n    A Komodo account is the organizational entity on the platform. Each account\n    has its own data subscriptions and a dedicated Komodo-managed Snowflake\n    warehouse. Every query and API operation is scoped to the selected account,\n    and data does not move between accounts.\n  identifiers:\n    account_id: UUID uniquely identifying the account\n    account_slug: human-readable account name\n  selection: komodo account set (interactive) / komodo account get / komodo account list\n\ncredentials_file:\n  path: ~/.komodo/credentials\n  format: INI-style named profiles\n  override_env: KOMODO_CREDENTIALS_PATH\n  profiles:\n    default: >-\n      Written by\
  \ `komodo login` and `komodo account set`. Carries token,\n      token_expiration, account_id and account_slug.\n    named: >-\n      User-created profiles carrying client_id, client_secret, account_id and\n      account_slug. Named profiles support M2M credentials only, not JWTs.\n\nrules:\n  - Only one authentication method may be used at a time.\n  - JWT and explicit M2M credentials both require an account_id parameter.\n  - Profiles cannot be combined with account_id — the profile already carries it.\n  - jwt and client_id/client_secret cannot be mixed.\n\nenvironments:\n  - {name: production, default: true, public: true}\n  - {name: integration, public: false, requires: komodo-internal-tools plugin}\n  - {name: development, public: false, requires: komodo-internal-tools plugin}\n\nscopes:\n  published: false\n  note: >-\n    Komodo does not publish an OAuth scope or permission reference. App-level\n    authorization is expressed as grantable roles on Komodo Apps (see the\n    App\
  \ Builder sharing tools) and RBAC/FGA on app and secret resources.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komodo-health/refs/heads/main/authentication/komodo-health-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Healthcare
- Health Data
- Life Sciences
- Real-World Data
- Healthcare Analytics
- Artificial Intelligence
- Data
- Snowflake
- MCP
---
