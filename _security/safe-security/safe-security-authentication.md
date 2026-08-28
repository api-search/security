---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Safe Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: SAFE Security declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SAFE Security
provider_slug: safe-security
scheme_count: 2
schemes:
- description: HTTP Basic with an API username and API password generated in the SAFE application under Settings > API Credentials. Used only to call the token endpoint; it is not accepted on resource endpoints.
  header: Authorization
  id: basicAuth
  in: header
  purpose: bootstrap
  scheme: basic
  type: http
- bearer_format: JWT-style access token
  description: 'The access token returned by POST /api/v3/auth, sent as ''Authorization: Bearer {{safe-bearer-token}}'' on every subsequent call.'
  header: Authorization
  id: bearerAuth
  in: header
  purpose: resource-access
  scheme: bearer
  type: http
slug: safe-security-authentication
source_filename: safe-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.safe.security/docs/accessing-safe-apis\nname: SAFE REST API authentication\ndocs:\n- https://docs.safe.security/docs/accessing-safe-apis\n- https://docs.safe.security/docs/api-credentials\nnote: >-\n  Derived from the published documentation rather than from a securitySchemes block:\n  SAFE's Swagger reference is served inside the authenticated application and its\n  spec JSON is not retrievable anonymously (see conformance/ evidence), so the auth\n  model below is transcribed from SAFE's own public docs pages.\nschemes:\n- id: basicAuth\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  purpose: bootstrap\n  description: >-\n    HTTP Basic with an API username and API password generated in the SAFE\n    application under Settings > API Credentials. Used only to call the token\n    endpoint; it is not accepted on resource endpoints.\n- id: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format:\
  \ JWT-style access token\n  in: header\n  header: Authorization\n  purpose: resource-access\n  description: >-\n    The access token returned by POST /api/v3/auth, sent as\n    'Authorization: Bearer {{safe-bearer-token}}' on every subsequent call.\ntoken_endpoint:\n  operation: POST /api/v3/auth\n  request_auth: basicAuth\n  returns: accessToken\n  ttl: 1h\n  ttl_source: >-\n    \"You can now use any of the SAFE APIs for the next hour. The access token will\n    expire, so it may be necessary to repeat this process.\" - Accessing SAFE APIs\ncredential_management:\n  created_in: SAFE application UI, Settings > API Credentials\n  self_service: true\n  roles_permitted:\n  - Admin\n  shown_once: true\n  permissions: read/write\n  permission_granularity: none\n  expiry_configurable: true\n  expiry_options:\n  - 30 days\n  - 60 days\n  - 90 days\n  - 180 days\n  - 365 days\n  - custom 1-365 days\n  max_validity_setting: Settings > System Setup > Security\n  revocation: Delete the credential\
  \ from Settings > API Credentials\n  note: >-\n    Per SAFE's own FAQ, \"API keys are only available for the Admin role in SAFE...\n    These keys have both read/write permissions.\" There are no read-only API\n    credentials and no scope selection, so any integration holding a SAFE API\n    credential holds full read/write authority over the tenant. Lowering the\n    tenant-wide maximum validity retroactively shortens the expiry of credentials\n    already issued, and that shortening cannot be undone.\noauth2: false\nopenid_connect:\n  api: false\n  console: true\n  note: >-\n    OAuth 2.0 / OIDC is not used for API authentication. SSO to the SAFE application\n    itself is supported for human users via SAML/OIDC with Microsoft Entra ID, Okta,\n    AD FS, Duo and OneLogin (docs.safe.security/docs/generic-sso-parameters); it does\n    not apply to REST API credentials.\nmtls: false\napi_keys: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safe-security/refs/heads/main/authentication/safe-security-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Cyber Risk Quantification
- Third-Party Risk Management
- Continuous Threat Exposure Management
- AI Security Posture Management
- Risk Management
- Governance Risk and Compliance
- FAIR
- Vulnerability Management
---
