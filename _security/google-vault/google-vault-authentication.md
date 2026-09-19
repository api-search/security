---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-vault-exports-api-openapi.yml
  format: yaml
  label: Google Vault Exports API
  slug: google-vault-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-exports-api-openapi.yml
- filename: google-vault-heldaccounts-api-openapi.yml
  format: yaml
  label: Google Vault HeldAccounts API
  slug: google-vault-heldaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-heldaccounts-api-openapi.yml
- filename: google-vault-holds-api-openapi.yml
  format: yaml
  label: Google Vault Holds API
  slug: google-vault-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-holds-api-openapi.yml
- filename: google-vault-matters-api-openapi.yml
  format: yaml
  label: Google Vault Matters API
  slug: google-vault-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-matters-api-openapi.yml
- filename: google-vault-operations-api-openapi.yml
  format: yaml
  label: Google Vault Operations API
  slug: google-vault-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-operations-api-openapi.yml
- filename: google-vault-saved-queries-api-openapi.yml
  format: yaml
  label: Google Vault Saved Queries API
  slug: google-vault-saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-saved-queries-api-openapi.yml
auth_types:
- oauth2
description: Every Vault API method requires an OAuth 2.0 access token; there is no API-key or unauthenticated path. Vault is an admin surface, so the token must belong to a Google Workspace user who holds Vault privileges (or to a service account with domain-wide delegation impersonating one). The authorization server is accounts.google.com, whose OIDC and RFC 8414 metadata are saved verbatim under well-known/.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Vault Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Vault secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Vault
provider_slug: google-vault
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  header: 'Authorization: Bearer <access token>'
  in: header
  name: googleOAuth
  sources:
  - openapi/google-vault-matters-api-openapi.yml
  - discovery/google-vault-discovery-v1.json
  type: oauth2
slug: google-vault-authentication
source_filename: google-vault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.google.com/workspace/vault/auth\ndocs: https://developers.google.com/workspace/vault/auth\nreferences:\n  - https://developers.google.com/workspace/vault/auth\n  - https://developers.google.com/workspace/guides/auth-overview\n  - https://developers.google.com/identity/protocols/oauth2\n  - https://developers.google.com/workspace/vault/troubleshoot-authentication-authorization\n  - well-known/google-vault-openid-configuration.json\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_supported: false\n  anonymous_access: false\n  scopes: 2\ndescription: >-\n  Every Vault API method requires an OAuth 2.0 access token; there is no API-key or\n  unauthenticated path. Vault is an admin surface, so the token must belong to a Google\n  Workspace user who holds Vault privileges (or to a service account with domain-wide\n  delegation impersonating one). The authorization server is accounts.google.com,\
  \ whose OIDC\n  and RFC 8414 metadata are saved verbatim under well-known/.\nschemes:\n  - name: googleOAuth\n    type: oauth2\n    in: header\n    header: 'Authorization: Bearer <access token>'\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        scopes: 2\n    sources:\n      - openapi/google-vault-matters-api-openapi.yml\n      - discovery/google-vault-discovery-v1.json\ncredential_types:\n  - kind: oauth-user\n    name: OAuth 2.0 client (installed / web app)\n    consent: https://developers.google.com/workspace/guides/configure-oauth-consent\n    note: >-\n      The Java and Python quickstarts both use a downloaded OAuth client\n      (credentials.json) and an interactive consent step.\n  - kind: service-account-dwd\n    name: Service account with domain-wide delegation\n    note: >-\n      Server-to-server access impersonates a Workspace user who has Vault\
  \ privileges. A raw\n      service account identity with no impersonation has no Vault data of its own.\n    docs: https://developers.google.com/workspace/guides/create-credentials\n  - kind: api-key\n    supported: false\n    note: >-\n      Vault carries only user data, so the api key path Google offers for public data APIs\n      does not apply. The Discovery document's global `key` parameter exists on every Google\n      API but does not satisfy the method's scopes[] requirement.\nauthorization:\n  model: >-\n    OAuth scope AND Google Workspace Vault privilege. Holding the ediscovery scope is not\n    sufficient — the acting user must also be granted the relevant Vault privileges in the\n    Admin console, and matters are further gated per-matter by MatterPermission.\n  scopes_detail: scopes/google-vault-scopes.yml\n  per_matter: >-\n    matters.addPermissions / matters.removePermissions manage collaborator access on a single\n    matter via the MatterPermission resource, so visibility\
  \ is scoped per matter and not only\n    per user.\nfailure_modes:\n  - status: 401\n    meaning: The access token is invalid or expired.\n    remedy: Refresh the token and retry.\n    source: https://developers.google.com/workspace/vault/guides/errors\n  - status: 404\n    meaning: >-\n      The specified resource was not found — returned when the request names a matter, hold or\n      account that does not exist. Verbatim from the provider's error guide; the guide does not\n      document a 403, so permission failures are not separately described there.\n    source: https://developers.google.com/workspace/vault/guides/errors\nconsent_and_setup_failures:\n  source: https://developers.google.com/workspace/vault/troubleshoot-authentication-authorization\n  documented:\n    - symptom: This app isn't verified\n      cause: The app requests scopes over sensitive user data and has not completed verification.\n    - symptom: File not found error for credentials.json\n      cause: Desktop-application\
  \ credentials were never created or are not in the working directory.\n    - symptom: Token has been expired or revoked\n      cause: The access/refresh token from Google's authorization server is no longer valid.\n    - symptom: 'JavaScript: origin_mismatch / idpiframe_initialization_failed'\n      cause: Authorized JavaScript origin mismatch, or third-party cookies disabled for accounts.google.com.\nauthorization_server:\n  issuer: https://accounts.google.com\n  openid_configuration: well-known/google-vault-openid-configuration.json\n  oauth_authorization_server: well-known/google-vault-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/authentication/google-vault-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- eDiscovery
- Legal Hold
- Information Governance
- Compliance
- Archiving
- Retention
- Google Workspace
- Audit
---
