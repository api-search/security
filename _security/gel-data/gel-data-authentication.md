---
api_key_in: []
auth_types:
- http
- oauth2
- webauthn
- magic-link
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gel Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gel Data secures its APIs with http, oauth2, webauthn, magic-link, and apiKey across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gel Data
provider_slug: gel-data
scheme_count: 7
schemes:
- applies_to: database protocol / client libraries
  name: gel-connection-scram
  scheme: scram-sha-256
  source: https://docs.geldata.com/reference/reference/protocol
  type: http
- applies_to: Gel Cloud instances and the HTTP endpoints
  in: header
  name: gel-cloud-secret-key
  note: Bearer secret key generated via the CLI (gel cloud secretkey create)
  source: https://docs.geldata.com/reference/running/http
  type: apiKey
- applies_to: instance TLS; server presents a TLS cert, clients may pin/verify
  name: gel-mtls
  source: https://docs.geldata.com/reference/running/configuration
  type: mutualTLS
- applies_to: Gel Auth extension — social login providers (Google, GitHub, Apple, Azure, Discord, Slack) via OAuth 2.0 authorization code flow
  name: gel-auth-oauth
  source: https://docs.geldata.com/reference/auth/oauth
  type: oauth2
- applies_to: Gel Auth extension — email/password sign-up and sign-in with PKCE
  name: gel-auth-email-password
  scheme: email-password
  source: https://docs.geldata.com/reference/auth/email_password
  type: http
- applies_to: Gel Auth extension — passwordless email magic links
  name: gel-auth-magic-link
  source: https://docs.geldata.com/reference/auth/magic_link
  type: magic-link
- applies_to: Gel Auth extension — passkeys / WebAuthn
  name: gel-auth-webauthn
  source: https://docs.geldata.com/reference/auth/webauthn
  type: webauthn
slug: gel-data-authentication
source_filename: gel-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.geldata.com/reference/auth\ndocs: https://docs.geldata.com/reference/auth/http\nsummary:\n  types: [http, oauth2, webauthn, magic-link, apiKey]\n  notes: Two distinct auth surfaces — (1) database connection auth via SCRAM/mTLS/secret\n    keys for clients and the CLI, and (2) the Gel Auth extension, a built-in identity\n    provider for application end-users.\nschemes:\n- name: gel-connection-scram\n  type: http\n  scheme: scram-sha-256\n  applies_to: database protocol / client libraries\n  source: https://docs.geldata.com/reference/reference/protocol\n- name: gel-cloud-secret-key\n  type: apiKey\n  in: header\n  applies_to: Gel Cloud instances and the HTTP endpoints\n  note: Bearer secret key generated via the CLI (gel cloud secretkey create)\n  source: https://docs.geldata.com/reference/running/http\n- name: gel-mtls\n  type: mutualTLS\n  applies_to: instance TLS; server presents a TLS cert, clients may pin/verify\n\
  \  source: https://docs.geldata.com/reference/running/configuration\n- name: gel-auth-oauth\n  type: oauth2\n  applies_to: Gel Auth extension — social login providers (Google, GitHub, Apple, Azure,\n    Discord, Slack) via OAuth 2.0 authorization code flow\n  source: https://docs.geldata.com/reference/auth/oauth\n- name: gel-auth-email-password\n  type: http\n  scheme: email-password\n  applies_to: Gel Auth extension — email/password sign-up and sign-in with PKCE\n  source: https://docs.geldata.com/reference/auth/email_password\n- name: gel-auth-magic-link\n  type: magic-link\n  applies_to: Gel Auth extension — passwordless email magic links\n  source: https://docs.geldata.com/reference/auth/magic_link\n- name: gel-auth-webauthn\n  type: webauthn\n  applies_to: Gel Auth extension — passkeys / WebAuthn\n  source: https://docs.geldata.com/reference/auth/webauthn\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gel-data/refs/heads/main/authentication/gel-data-authentication.yml
summary_line: http/oauth2/webauthn/magic-link/apiKey · 7 schemes
tags:
- Company
- Open Source
- Database
- PostgreSQL
- Graph Database
- GraphQL
- Authentication
- Artificial Intelligence
- Vector Database
- Developer Tools
---
