---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accredify0604-nexus-auth-openapi.yaml
  format: yaml
  label: Accredify Nexus API
  slug: accredify0604-nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-nexus-auth-openapi.yaml
- filename: accredify0604-dashboard-v1-openapi.yaml
  format: yaml
  label: Accredify Dashboard API
  slug: accredify0604-dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-dashboard-v1-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accredify0604 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Accredify secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Accredify
provider_slug: accredify0604
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT Authorization header using the Bearer scheme. Example: ''Authorization: Bearer {token}'''
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/accredify0604-dashboard-v1-openapi.yaml
  - openapi/accredify0604-dashboard-v2-openapi.yaml
  type: http
- description: OAuth2 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 20
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/accredify0604-nexus-auth-openapi.yaml
  - openapi/accredify0604-nexus-verification-openapi.yaml
  - openapi/accredify0604-nexus-workflow-openapi.yaml
  type: oauth2
slug: accredify0604-authentication
source_filename: accredify0604-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.nexus.accredify.io/auth.yaml, https://docs.dashboard.accredify.io/v1.yaml, https://docs.dashboard.accredify.io/v2.yaml\n  (fetched 2026-09-06); mirrored to openapi/\ndocs: https://docs.nexus.accredify.io/auth.html\nnote: 'Accredify runs TWO different auth models and a client must pick the right one per API family. Nexus\n  (nexus.accredify.io) uses OAuth 2.0 client credentials against POST /oauth/token with an application/x-www-form-urlencoded\n  body (grant_type=client_credentials, client_id, client_secret, and a space-separated scope string),\n  returning a Bearer token with expires_in 31536000 — one year. The Dashboard (dashboard.accredify.io)\n  uses an OAuth 2.0 authorization-code flow (GET /v1/oauth/redirect, POST /v1/oauth/grant, POST /v1/oauth/refresh)\n  yielding an unscoped bearer JWT. Nexus additionally mints long-lived per-user API tokens whose plaintext\n  secret is returned exactly once and which\
  \ are auto-revoked when the subject user is locked. A third,\n  separate authorization surface exists for credential issuance: the OID4VCI authorization server at https://nexus.accredify.io/.well-known/oauth-authorization-server,\n  which advertises the pre-authorized_code grant with anonymous access and S256 PKCE — that is the wallet\n  flow, not the API flow.'\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Authorization header using the Bearer scheme. Example: ''Authorization: Bearer {token}'''\n  sources:\n  - openapi/accredify0604-dashboard-v1-openapi.yaml\n  - openapi/accredify0604-dashboard-v2-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 20\n  description: OAuth2 client credentials flow\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-verification-openapi.yaml\n\
  \  - openapi/accredify0604-nexus-workflow-openapi.yaml\ntoken_endpoints:\n- api: Accredify Nexus API\n  url: https://nexus.accredify.io/oauth/token\n  grant: client_credentials\n  body: application/x-www-form-urlencoded\n  expires_in: 31536000\n- api: Accredify Dashboard API\n  url: https://dashboard.accredify.io/api/v1/oauth/grant\n  grant: authorization_code\n  refresh: https://dashboard.accredify.io/api/v1/oauth/refresh\n- api: OID4VCI credential issuance\n  url: https://nexus.accredify.io/oid4vci/tokens\n  grant: urn:ietf:params:oauth:grant-type:pre-authorized_code\n  source: https://nexus.accredify.io/.well-known/oauth-authorization-server\n  note: Wallet/holder flow for issuing mso_mdoc credentials, not the REST API auth path.\nscopes_artifact: scopes/accredify0604-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/authentication/accredify0604-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Verifiable Credentials
- Digital Credentials
- Identity
- Document Verification
- Credentialing
- Education
- Healthcare
- Trust
- OpenBadges
- OID4VCI
- Singapore
---
