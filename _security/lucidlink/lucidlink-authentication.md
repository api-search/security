---
api_key_in: []
api_specs:
- filename: lucidlink-service-api.json
  format: json
  label: LucidLink Service API
  slug: lucidlink-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidlink/refs/heads/main/openapi/lucidlink-service-api.json
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Lucidlink Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LucidLink secures its APIs with oauth2 and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LucidLink
provider_slug: lucidlink
scheme_count: 3
schemes:
- api: LucidLink Service API v1
  applied: 'globally — the document carries a top-level `security` block of `[{standard: []}]`'
  credential_issuance: Not self-service. "The credentials are provided upon request sent to support+ticket@lucidlink.com or by visiting https://support.lucidlink.com/hc/en-us." (info.description of the published Swagger document.)
  declared_in: openapi/lucidlink-service-api.json
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.lucidlink.com/oauth2/token
  name: standard
  request_header: 'Authorization: <access_token>'
  request_header_note: LucidLink's own published example sends the raw access token with no `Bearer` prefix on this API. Recorded as published; it is not RFC 6750 form.
  sources:
  - openapi/lucidlink-service-api.json
  token_request: 'POST https://auth.lucidlink.com/oauth2/token with `Authorization: Basic base64(CLIENT_ID:CLIENT_SECRET)`, `Content-Type: application/x-www-form-urlencoded`, body `grant_type=client_credentials`.'
  type: oauth2
- api: LucidLink Management API v1 (self-hosted) and Web Service API v2
  declared_in: documentation only — no published specification
  display: Credentials are shown only once, at generation or rotation.
  issuance: Workspace admins create service accounts in the "Service Accounts" tab of workspace settings in the web or desktop app. Available to Business and Enterprise tiers; not separately billed.
  name: service-account-bearer
  request_header: 'Authorization: Bearer <service key>'
  revocation: Deleting a service account immediately invalidates all of its credentials.
  rotation: A service account can hold multiple secret keys, so a new key can be issued and the old one retired without interrupting service. `lucid rotate-credentials` (build 3.7.8468) rotates the key used by the desktop daemon in place, without remounting the filespace.
  scheme: bearer
  scope: IMPORTANT — for the initial release a service account "inherits the full permissions/scope of a workspace administrator, granting access to all available API functionalities". There is no least-privilege option on a standard service account.
  sources:
  - https://support.lucidlink.com/hc/en-us/articles/40222074543757-Getting-Started-with-Service-Accounts-API-Authentication
  - https://support.lucidlink.com/hc/en-us/articles/40222376164365-Best-Practices-Operating-the-LucidLink-API-Container
  token_prefix: 'sa_live:'
  token_prefix_source: LucidLink's published lucidlink-mcp README
  transport_warning: The Management API container serves plain HTTP on port 3003. LucidLink's own best-practices article requires putting it behind a TLS-terminating reverse proxy so the bearer token is never sent in clear text, and restricting the port to trusted internal systems.
  type: http
- api: LucidLink Management API v1
  availability: All plans including Trial.
  name: collaborator-service-account
  note: No UI in this beta; Collaborator Service Accounts are created and managed through the LucidLink API itself.
  purpose: Scope automation to specific LucidLink folders and filespaces "without handing out full administrator credentials" — the least-privilege answer to the scope gap above.
  scheme: bearer
  since: build 3.7.8584 (2026-08-08)
  sources:
  - https://support.lucidlink.com/hc/en-us/articles/48014583746573-Collaborator-Service-Accounts-Beta
  status: beta
  type: http
slug: lucidlink-authentication
source_filename: lucidlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  openapi/lucidlink-service-api.json (securityDefinitions + info.description worked example),\n  https://support.lucidlink.com/hc/en-us/articles/40222074543757-Getting-Started-with-Service-Accounts-API-Authentication,\n  https://support.lucidlink.com/hc/en-us/articles/48014583746573-Collaborator-Service-Accounts-Beta,\n  and the published lucidlink-mcp 0.3.0 README\ndocs: https://support.lucidlink.com/hc/en-us/articles/40222074543757-Getting-Started-with-Service-Accounts-API-Authentication\nsummary:\n  types: [oauth2, http-bearer]\n  oauth2_flows: [clientCredentials]\n  api_keys: false\n  mtls: false\n  openid_connect: false\n  note: >-\n    Two distinct models across three APIs. The public Service API uses an OAuth2\n    client-credentials grant; the self-hosted Management API and the v2 web service use a\n    service-account secret key as a bearer token. There is no user-delegated OAuth flow and\n    no OIDC anywhere.\n\
  schemes:\n- name: standard\n  api: LucidLink Service API v1\n  type: oauth2\n  declared_in: openapi/lucidlink-service-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.lucidlink.com/oauth2/token\n    scopes: 0\n  applied: >-\n    globally — the document carries a top-level `security` block of\n    `[{standard: []}]`\n  token_request: >-\n    POST https://auth.lucidlink.com/oauth2/token with\n    `Authorization: Basic base64(CLIENT_ID:CLIENT_SECRET)`,\n    `Content-Type: application/x-www-form-urlencoded`, body `grant_type=client_credentials`.\n  request_header: 'Authorization: <access_token>'\n  request_header_note: >-\n    LucidLink's own published example sends the raw access token with no `Bearer` prefix on\n    this API. Recorded as published; it is not RFC 6750 form.\n  credential_issuance: >-\n    Not self-service. \"The credentials are provided upon request sent to\n    support+ticket@lucidlink.com or by visiting https://support.lucidlink.com/hc/en-us.\"\
  \n    (info.description of the published Swagger document.)\n  sources: [openapi/lucidlink-service-api.json]\n- name: service-account-bearer\n  api: LucidLink Management API v1 (self-hosted) and Web Service API v2\n  type: http\n  scheme: bearer\n  declared_in: documentation only — no published specification\n  request_header: 'Authorization: Bearer <service key>'\n  token_prefix: 'sa_live:'\n  token_prefix_source: LucidLink's published lucidlink-mcp README\n  issuance: >-\n    Workspace admins create service accounts in the \"Service Accounts\" tab of workspace\n    settings in the web or desktop app. Available to Business and Enterprise tiers; not\n    separately billed.\n  rotation: >-\n    A service account can hold multiple secret keys, so a new key can be issued and the old\n    one retired without interrupting service. `lucid rotate-credentials` (build 3.7.8468)\n    rotates the key used by the desktop daemon in place, without remounting the filespace.\n  display: Credentials are\
  \ shown only once, at generation or rotation.\n  revocation: Deleting a service account immediately invalidates all of its credentials.\n  scope: >-\n    IMPORTANT — for the initial release a service account \"inherits the full\n    permissions/scope of a workspace administrator, granting access to all available API\n    functionalities\". There is no least-privilege option on a standard service account.\n  transport_warning: >-\n    The Management API container serves plain HTTP on port 3003. LucidLink's own\n    best-practices article requires putting it behind a TLS-terminating reverse proxy so the\n    bearer token is never sent in clear text, and restricting the port to trusted internal\n    systems.\n  sources:\n  - https://support.lucidlink.com/hc/en-us/articles/40222074543757-Getting-Started-with-Service-Accounts-API-Authentication\n  - https://support.lucidlink.com/hc/en-us/articles/40222376164365-Best-Practices-Operating-the-LucidLink-API-Container\n- name: collaborator-service-account\n\
  \  api: LucidLink Management API v1\n  type: http\n  scheme: bearer\n  status: beta\n  since: build 3.7.8584 (2026-08-08)\n  purpose: >-\n    Scope automation to specific LucidLink folders and filespaces \"without handing out full\n    administrator credentials\" — the least-privilege answer to the scope gap above.\n  availability: All plans including Trial.\n  note: >-\n    No UI in this beta; Collaborator Service Accounts are created and managed through the\n    LucidLink API itself.\n  sources:\n  - https://support.lucidlink.com/hc/en-us/articles/48014583746573-Collaborator-Service-Accounts-Beta\nend_user_identity:\n  sso:\n    protocol: SAML 2.0\n    providers: [Okta, Microsoft Entra ID / Azure AD, Google Workspace, OneLogin]\n    docs: https://support.lucidlink.com/hc/en-us/sections/31125114361741-Single-Sign-On-SAML\n  provisioning:\n    protocol: SCIM 2.0\n    docs: https://support.lucidlink.com/hc/en-us/articles/38861860730637-Understanding-SCIM-Integration-in-LucidLink\n    note:\
  \ Requires SSO first. Google Workspace group provisioning is not supported.\n  mfa:\n    supported: true\n    scope: Two-factor authentication for non-SSO users\n    docs: https://support.lucidlink.com/hc/en-us/articles/44137711794189-Configure-Multi-Factor-Authentication-for-your-User-Account\n  proxy_auth:\n    kerberos: 'Windows only, since build 3.7.8468 (2026-07-11)'\ngaps:\n- No OAuth2 scopes are declared or documented — a client credential is all-or-nothing across domains, filespaces and billing including setPaymentDetails.\n- No RFC 8414 authorization-server metadata and no OIDC discovery document at auth.lucidlink.com (both probed, both 404).\n- No 401 or 403 response is declared on any operation in the published Swagger document, although the live API returns 401.\n- Standard service accounts carry full workspace-admin authority; least privilege is only available through the Collaborator Service Accounts beta.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidlink/refs/heads/main/authentication/lucidlink-authentication.yml
summary_line: oauth2/http-bearer · 3 schemes
tags:
- Company
- Cloud Storage
- File Streaming
- File Collaboration
- Media and Entertainment
- Object Storage
- Developer Platform
- MCP
- Agentic AI
- Zero-Knowledge Encryption
- Identity and Access Management
---
