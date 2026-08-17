---
api_key_in: []
auth_types: []
description: 'How callers authenticate to the Komodo Health platform. Komodo supports two mutually exclusive modes: interactive web login (OAuth 2.0 Device Authorization Flow, yielding a JWT) and machine-to-machine service-principal credentials (client_id / client_secret). Every call is scoped to a Komodo account, each of which maps to a dedicated Komodo-managed Snowflake warehouse.

  UPGRADED 2026-08-15: the 2026-07-19 round could only document these schemes from prose because Komodo publishes no OpenAPI. The Kong gateway at api.komodohealth.com answers every anonymous request with `WWW-Authenticate: Bearer realm="auth.komodohealth.com", error="invalid_token"`, and that authorization server publishes a full anonymous OIDC discovery document. The endpoints, grants, PKCE methods, signing algorithms and token endpoint auth methods below are now machine-read from the provider rather than inferred, and they corroborate the documented flows exactly (the device authorization endpoint confirms `komodo login`; client_credentials confirms service principals).'
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
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: >-\n  https://docs.komodohealth.com/guides-tutorials/guides/2-authentication and —\n  new on 2026-08-15 — the authorization server's own discovery documents at\n  https://auth.komodohealth.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server, saved verbatim under well-known/.\ndescription: >-\n  How callers authenticate to the Komodo Health platform. Komodo supports two\n  mutually exclusive modes: interactive web login (OAuth 2.0 Device\n  Authorization Flow, yielding a JWT) and machine-to-machine service-principal\n  credentials (client_id / client_secret). Every call is scoped to a Komodo\n  account, each of which maps to a dedicated Komodo-managed Snowflake warehouse.\n\n  UPGRADED 2026-08-15: the 2026-07-19 round could only document these schemes\n  from prose because Komodo publishes no OpenAPI. The Kong gateway at\n  api.komodohealth.com answers every anonymous request with\n  `WWW-Authenticate:\
  \ Bearer realm=\"auth.komodohealth.com\", error=\"invalid_token\"`,\n  and that authorization server publishes a full anonymous OIDC discovery\n  document. The endpoints, grants, PKCE methods, signing algorithms and token\n  endpoint auth methods below are now machine-read from the provider rather than\n  inferred, and they corroborate the documented flows exactly (the device\n  authorization endpoint confirms `komodo login`; client_credentials confirms\n  service principals).\ndocs: https://docs.komodohealth.com/guides-tutorials/guides/2-authentication\n\nauthorization_server:\n  issuer: https://auth.komodohealth.com/\n  discovery:\n    openid_configuration: https://auth.komodohealth.com/.well-known/openid-configuration\n    oauth_authorization_server: https://auth.komodohealth.com/.well-known/oauth-authorization-server\n    status: 200\n    probed: '2026-08-15'\n    files:\n      - well-known/komodo-health-openid-configuration.json\n      - well-known/komodo-health-oauth-authorization-server.json\n\
  \      - well-known/komodo-health-jwks.json\n  backed_by: Auth0 (auth0.com grant-type extensions present in grant_types_supported)\n  ownership_note: >-\n    auth.komodohealth.com is a Komodo-owned hostname and the issuer claim is\n    https://auth.komodohealth.com/, so this authorization server belongs to\n    Komodo Health even though the underlying identity platform is Auth0.\n  endpoints:\n    authorization: https://auth.komodohealth.com/authorize\n    token: https://auth.komodohealth.com/oauth/token\n    device_authorization: https://auth.komodohealth.com/oauth/device/code\n    userinfo: https://auth.komodohealth.com/userinfo\n    jwks: https://auth.komodohealth.com/.well-known/jwks.json\n    revocation: https://auth.komodohealth.com/oauth/revoke\n    registration: https://auth.komodohealth.com/oidc/register\n    mfa_challenge: https://auth.komodohealth.com/mfa/challenge\n    backchannel_authentication: https://auth.komodohealth.com/bc-authorize\n    global_token_revocation: https://auth.komodohealth.com/oauth/global-token-revocation/connection/{connectionName}\n\
  \  grant_types_supported:\n    - client_credentials\n    - authorization_code\n    - refresh_token\n    - password\n    - implicit\n    - urn:ietf:params:oauth:grant-type:device_code\n    - urn:ietf:params:oauth:grant-type:token-exchange\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n    - http://auth0.com/oauth/grant-type/password-realm\n    - http://auth0.com/oauth/grant-type/passwordless/otp\n    - http://auth0.com/oauth/grant-type/mfa-oob\n    - http://auth0.com/oauth/grant-type/mfa-otp\n    - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  subject_types_supported: [public]\n  backchannel_logout_supported: true\n  scopes_supported_detail: scopes/komodo-health-scopes.yml\n\nschemes:\n  - id: web_login\n    type:\
  \ oauth2\n    flow: device_authorization\n    rfc: RFC 8628\n    description: >-\n      Browser-based OAuth flow for interactive users. Started with `komodo\n      login`; opens the browser, then persists the JWT and refresh token to the\n      [default] profile in ~/.komodo/credentials. Intended for individual,\n      manual use.\n    token_type: JWT\n    token_command: komodo jwt\n    persisted: true\n    persisted_to: ~/.komodo/credentials\n    note: >-\n      If no credentials are found the SDK triggers a web login automatically,\n      but those credentials are in-memory only and are not written to disk.\n  - id: service_principal\n    type: oauth2\n    flow: client_credentials\n    description: >-\n      Machine-to-machine authentication for automation, CI/CD and services.\n      Service principals are created with `komodo service-principal create`,\n      which returns a client_id and client_secret. No user interaction required.\n    credentials: [client_id, client_secret]\n   \
  \ requires: account_id (or a named profile that carries it)\n    management_commands:\n      - komodo service-principal create --name \"<name>\" --description \"<desc>\"\n      - komodo service-principal list\n      - komodo service-principal delete <SERVICE_PRINCIPAL_ID>\n  - id: explicit_jwt\n    type: http\n    scheme: bearer\n    description: >-\n      A JWT obtained from `komodo jwt` may be passed directly into the SDK\n      alongside an account_id. In-memory only.\n\naccount_scoping:\n  required: true\n  description: >-\n    A Komodo account is the organizational entity on the platform. Each account\n    has its own data subscriptions and a dedicated Komodo-managed Snowflake\n    warehouse. Every query and API operation is scoped to the selected account,\n    and data does not move between accounts.\n  identifiers:\n    account_id: UUID uniquely identifying the account\n    account_slug: human-readable account name\n  selection: komodo account set (interactive) / komodo account\
  \ get / komodo account list\n\ncredentials_file:\n  path: ~/.komodo/credentials\n  format: INI-style named profiles\n  override_env: KOMODO_CREDENTIALS_PATH\n  profiles:\n    default: >-\n      Written by `komodo login` and `komodo account set`. Carries token,\n      token_expiration, account_id and account_slug.\n    named: >-\n      User-created profiles carrying client_id, client_secret, account_id and\n      account_slug. Named profiles support M2M credentials only, not JWTs.\n\nrules:\n  - Only one authentication method may be used at a time.\n  - JWT and explicit M2M credentials both require an account_id parameter.\n  - Profiles cannot be combined with account_id — the profile already carries it.\n  - jwt and client_id/client_secret cannot be mixed.\n\nenvironments:\n  - {name: production, default: true, public: true}\n  - {name: integration, public: false, requires: komodo-internal-tools plugin}\n  - {name: development, public: false, requires: komodo-internal-tools plugin}\n\n\
  scopes:\n  published: partial\n  detail: scopes/komodo-health-scopes.yml\n  note: >-\n    UPGRADED 2026-08-15. The authorization server advertises 14 scopes in its\n    discovery document, but every one of them is a standard OpenID Connect\n    identity/claim scope (openid, profile, email, offline_access, name,\n    given_name, family_name, nickname, picture, created_at, identities, phone,\n    address, email_verified). Komodo advertises NO resource scopes for its own\n    API and publishes no scopes/permissions reference page. Platform\n    authorization is expressed as Komodo account membership plus RBAC/FGA\n    grantable roles on Komodo Apps and secrets (see the App Builder sharing\n    tools). Do not read the OIDC scope list as a Komodo permission model.\n"
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
