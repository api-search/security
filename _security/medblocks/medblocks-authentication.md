---
api_key_in: []
api_specs:
- filename: medblocks-platform-openapi.json
  format: json
  label: Medblocks Platform API
  slug: medblocks-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-platform-openapi.json
- filename: medblocks-public-site-openapi.json
  format: json
  label: Medblocks Public Site API
  slug: medblocks-public-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-public-site-openapi.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Medblocks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medblocks secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medblocks
provider_slug: medblocks
scheme_count: 3
schemes:
- applies_to: medblocks-platform-api
  bearerFormat: API key (mb_sk_live_...)
  description: Medblocks API key for server-side requests.
  failure_codes:
  - code: missing_api_key
    meaning: Authorization header is missing
    status: 401
  - code: invalid_api_key
    meaning: API key is invalid
    status: 401
  - code: expired_api_key
    meaning: API key is expired
    status: 401
  - code: insufficient_scope
    meaning: API key lacks the required scope
    status: 403
  - code: api_key_limit_exceeded
    meaning: organization has reached its active API key cap
    status: 429
  global: true
  key_prefixes:
  - environment: production
    prefix: mb_sk_live_
  - environment: sandbox
    note: minted by a Sandbox workspace; only sees sandbox-scoped sources
    prefix: mb_sk_sbx_
  - environment: any
    note: The MCP docs and the provider's own agent skill refer to the key generically as mb_sk_; live and sandbox are the two documented environment suffixes.
    prefix: mb_sk_
  name: BearerAuth
  provisioning: Dashboard > Settings > API Keys
  scheme: bearer
  sources:
  - openapi/medblocks-platform-openapi.json
  type: http
  workspace_binding: A key is bound to the workspace that minted it and cannot switch workspaces.
- additional_grants:
  - client_credentials
  - refresh_token
  applies_to: mcp
  dynamic_client_registration: https://app.medblocks.com/api/auth/oauth2/register
  flows:
    authorizationCode:
      authorizationUrl: https://app.medblocks.com/api/auth/oauth2/authorize
      pkce: S256
      refreshUrl: https://app.medblocks.com/api/auth/oauth2/token
      tokenUrl: https://app.medblocks.com/api/auth/oauth2/token
  name: MedblocksOAuth
  note: Not declared in the OpenAPI document. Discovered from the provider's RFC 8414 metadata and the RFC 9728 challenge the MCP endpoint returns.
  scopes_artifact: scopes/medblocks-scopes.yml
  sources:
  - https://app.medblocks.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: mcp
  claims:
  - sub
  - iss
  - aud
  - exp
  - iat
  - sid
  - scope
  - azp
  - email
  - email_verified
  - name
  - picture
  - family_name
  - given_name
  id_token_signing_alg:
  - EdDSA
  name: MedblocksOIDC
  openIdConnectUrl: https://app.medblocks.com/.well-known/openid-configuration
  sources:
  - https://app.medblocks.com/.well-known/openid-configuration
  type: openIdConnect
slug: medblocks-authentication
source_filename: medblocks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://medblocks.com/docs/mcp, https://medblocks.com/docs/security-and-compliance,\n  https://medblocks.com/docs/sandboxes, https://medblocks.com/docs/reference/errors,\n  https://app.medblocks.com/.well-known/oauth-authorization-server,\n  openapi/medblocks-platform-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  note: >-\n    Two distinct authentication surfaces. The REST Medblocks Platform API is bearer API key\n    only — that is the single securityScheme in the contract, applied globally. The hosted MCP\n    server at https://app.medblocks.com/mcp additionally accepts OAuth 2.1 / OIDC with a\n    consent screen, and will also accept the same mb_sk_ key as a bearer token for\n    non-interactive developer clients.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (mb_sk_live_...)\n  description: Medblocks API key for server-side requests.\n  applies_to:\
  \ medblocks-platform-api\n  global: true\n  sources:\n  - openapi/medblocks-platform-openapi.json\n  key_prefixes:\n  - prefix: mb_sk_live_\n    environment: production\n  - prefix: mb_sk_sbx_\n    environment: sandbox\n    note: minted by a Sandbox workspace; only sees sandbox-scoped sources\n  - prefix: mb_sk_\n    environment: any\n    note: >-\n      The MCP docs and the provider's own agent skill refer to the key generically as mb_sk_;\n      live and sandbox are the two documented environment suffixes.\n  provisioning: Dashboard > Settings > API Keys\n  workspace_binding: >-\n    A key is bound to the workspace that minted it and cannot switch workspaces.\n  failure_codes:\n  - {status: 401, code: missing_api_key, meaning: Authorization header is missing}\n  - {status: 401, code: invalid_api_key, meaning: API key is invalid}\n  - {status: 401, code: expired_api_key, meaning: API key is expired}\n  - {status: 403, code: insufficient_scope, meaning: API key lacks the required scope}\n\
  \  - {status: 429, code: api_key_limit_exceeded, meaning: organization has reached its active API key cap}\n- name: MedblocksOAuth\n  type: oauth2\n  applies_to: mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.medblocks.com/api/auth/oauth2/authorize\n      tokenUrl: https://app.medblocks.com/api/auth/oauth2/token\n      refreshUrl: https://app.medblocks.com/api/auth/oauth2/token\n      pkce: S256\n  additional_grants: [client_credentials, refresh_token]\n  dynamic_client_registration: https://app.medblocks.com/api/auth/oauth2/register\n  scopes_artifact: scopes/medblocks-scopes.yml\n  sources:\n  - https://app.medblocks.com/.well-known/oauth-authorization-server\n  note: >-\n    Not declared in the OpenAPI document. Discovered from the provider's RFC 8414 metadata and\n    the RFC 9728 challenge the MCP endpoint returns.\n- name: MedblocksOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://app.medblocks.com/.well-known/openid-configuration\n  applies_to:\
  \ mcp\n  id_token_signing_alg: [EdDSA]\n  claims: [sub, iss, aud, exp, iat, sid, scope, azp, email, email_verified, name, picture, family_name, given_name]\n  sources:\n  - https://app.medblocks.com/.well-known/openid-configuration\nupstream_authentication:\n  note: >-\n    Distinct from calling Medblocks. Medblocks itself authenticates to the EHRs and payers on\n    the customer's behalf. Patient-mediated sources use per-patient OAuth against the source's\n    portal; backend/bulk sources use SMART Backend Services with a customer-supplied private\n    key. Source client secrets and SMART private keys are configured server-side in Medblocks\n    under Configure connections, never in browser code.\n  docs: https://medblocks.com/docs/configure-connections\nsecret_handling:\n  rules:\n  - Keep MEDBLOCKS_API_KEY server-side only; the frontend calls your backend and your backend calls Medblocks.\n  - Never place an API key in a URL, prompt, tool argument, browser bundle or log.\n  - Webhook\
  \ signing secrets, source client secrets, SMART private keys and export-destination credentials are all server-side secrets.\n  - Do not log API keys, webhook secrets, bearer tokens, access tokens, or full FHIR resources.\n  docs: https://medblocks.com/docs/security-and-compliance\nrevocation:\n  api_key: Rotate or revoke from Dashboard > Settings > API Keys.\n  oauth: >-\n    Dashboard > Settings > MCP server revokes an AI assistant's access; already-issued access\n    expires within an hour.\n  webhook_secret: POST /webhooks/{id}/rotate-secret (api.rotateWebhookSecret).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/authentication/medblocks-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Health
- Healthcare
- FHIR
- openEHR
- Interoperability
- Electronic Health Records
- Patient Access
- Health Data
- SMART on FHIR
- Webhooks
- Model Context Protocol
- Company
---
