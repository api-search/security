---
api_key_in:
- cookie
- header
api_specs:
- filename: opaque-asset-configs-api-openapi.yml
  format: yaml
  label: OPAQUE Asset Configs API
  slug: opaque-asset-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-asset-configs-api-openapi.yml
- filename: opaque-auth-api-openapi.yml
  format: yaml
  label: OPAQUE Auth API
  slug: opaque-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-auth-api-openapi.yml
- filename: opaque-datasets-api-openapi.yml
  format: yaml
  label: OPAQUE Datasets API
  slug: opaque-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-datasets-api-openapi.yml
- filename: opaque-jobs-api-openapi.yml
  format: yaml
  label: OPAQUE Jobs API
  slug: opaque-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-jobs-api-openapi.yml
- filename: opaque-organizations-api-openapi.yml
  format: yaml
  label: OPAQUE Organizations API
  slug: opaque-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-organizations-api-openapi.yml
- filename: opaque-pinned-queries-api-openapi.yml
  format: yaml
  label: OPAQUE Pinned Queries API
  slug: opaque-pinned-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-pinned-queries-api-openapi.yml
- filename: opaque-predefined-query-templates-api-openapi.yml
  format: yaml
  label: OPAQUE Predefined Query Templates API
  slug: opaque-predefined-query-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-predefined-query-templates-api-openapi.yml
- filename: opaque-users-api-openapi.yml
  format: yaml
  label: OPAQUE Users API
  slug: opaque-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-users-api-openapi.yml
- filename: opaque-versioning-api-openapi.yml
  format: yaml
  label: OPAQUE Versioning API
  slug: opaque-versioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-versioning-api-openapi.yml
- filename: opaque-workflows-api-openapi.yml
  format: yaml
  label: OPAQUE Workflows API
  slug: opaque-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-workflows-api-openapi.yml
- filename: opaque-workspaces-api-openapi.yml
  format: yaml
  label: OPAQUE Workspaces API
  slug: opaque-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/openapi/opaque-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Opaque Authentication
name_suffix: Authentication
oauth_flows: []
overview: OPAQUE secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OPAQUE
provider_slug: opaque
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: Short-lived (10 minute) JSON Web Token that authenticates general API requests. Sent in the Authorization header using the Bearer scheme. Obtained by exchanging a refresh token at POST /{version}/auth/refresh-token (operationId refresh_user_tokens); the response field is accessToken. The spec description says the token is obtained from the /login and /register endpoints.
  name: sessionToken
  scheme: bearer
  sources:
  - openapi/opaque-platform-api-openapi.yml
  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/
  type: http
- description: The same session token supplied as a cookie instead of a header, for browser-originated calls such as downloading job results or logs.
  in: cookie
  name: sessionTokenCookie
  parameter: sessionTokenCookie
  sources:
  - openapi/opaque-platform-api-openapi.yml
  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/
  type: apiKey
- description: Long-lived refresh token, stored as an HttpOnly cookie, exchanged for new session tokens. Extracted from the base64-encoded API key issued in the web application. A missing cookie returns 400; an expired refresh token returns 401 and requires the user to log in again.
  in: cookie
  name: refreshTokenCookie
  parameter: refreshTokenCookie
  sources:
  - openapi/opaque-platform-api-openapi.yml
  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/
  type: apiKey
- description: A binary blob derived from the user's passkey, sent as a cookie. Required for operations that involve cryptographic key exchange or sensitive data — uploading data and retrieving job results. The spec description says it can be obtained from the /login and /register endpoints; the docs describe extracting it from the decoded API key.
  in: cookie
  name: userIdentitySecret
  parameter: userIdentitySecret
  sources:
  - openapi/opaque-platform-api-openapi.yml
  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/
  type: apiKey
slug: opaque-authentication
source_filename: opaque-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/opaque-platform-api-openapi.yml\ndocs: https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows: []\n  model: >-\n    Three credential types, all issued per user. A base64-encoded API key is copied from the\n    \"API Keys\" page of the OPAQUE web application after SSO login; decoding it yields a JSON\n    object containing a refresh_token and a user_identity_secret. The refresh token is exchanged\n    at POST /{version}/auth/refresh-token for a short-lived session token (JWT), which is then\n    sent as an Authorization: Bearer header. The user identity secret is sent as a cookie and is\n    required for cryptographic / sensitive-data operations such as data upload and result\n    retrieval.\n  sso_required: true\n  api_key_lifetime: 6 months\n  session_token_lifetime: 10 minutes\nschemes:\n- name:\
  \ sessionToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Short-lived (10 minute) JSON Web Token that authenticates general API requests. Sent in the\n    Authorization header using the Bearer scheme. Obtained by exchanging a refresh token at\n    POST /{version}/auth/refresh-token (operationId refresh_user_tokens); the response field is\n    accessToken. The spec description says the token is obtained from the /login and /register\n    endpoints.\n  sources:\n  - openapi/opaque-platform-api-openapi.yml\n  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/\n- name: sessionTokenCookie\n  type: apiKey\n  in: cookie\n  parameter: sessionTokenCookie\n  description: >-\n    The same session token supplied as a cookie instead of a header, for browser-originated calls\n    such as downloading job results or logs.\n  sources:\n  - openapi/opaque-platform-api-openapi.yml\n  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/\n\
  - name: refreshTokenCookie\n  type: apiKey\n  in: cookie\n  parameter: refreshTokenCookie\n  description: >-\n    Long-lived refresh token, stored as an HttpOnly cookie, exchanged for new session tokens.\n    Extracted from the base64-encoded API key issued in the web application. A missing cookie\n    returns 400; an expired refresh token returns 401 and requires the user to log in again.\n  sources:\n  - openapi/opaque-platform-api-openapi.yml\n  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/\n- name: userIdentitySecret\n  type: apiKey\n  in: cookie\n  parameter: userIdentitySecret\n  description: >-\n    A binary blob derived from the user's passkey, sent as a cookie. Required for operations that\n    involve cryptographic key exchange or sensitive data — uploading data and retrieving job\n    results. The spec description says it can be obtained from the /login and /register endpoints;\n    the docs describe extracting it from the decoded API key.\n\
  \  sources:\n  - openapi/opaque-platform-api-openapi.yml\n  - https://docs.opaque.co/en/latest/public_guide/developers/rest_api/authentication/\ndefault_security:\n- sessionToken\n- refreshTokenCookie\nidentity:\n  sso: required\n  providers_documented:\n  - Microsoft Entra ID\n  - Okta\n  docs:\n  - https://docs.opaque.co/en/latest/public_guide/deployment/common_configurations/enable_entra_sso_for_opaque/\n  - https://docs.opaque.co/en/latest/public_guide/deployment/common_configurations/enable_okta_sso_for_opaque/\n  passkeys: >-\n    The API exposes create_passkey_from_password (POST /{version}/auth/create-passkey-from-password)\n    and get_user_keys (GET /{version}/user/keys); the user identity secret is derived from the\n    user's passkey.\nnotes:\n- No OAuth 2.0 or OpenID Connect security scheme is declared in the OpenAPI, and no scope surface\n  is published, so no scopes/ artifact is emitted. SSO is enforced at the web application layer\n  (Entra ID / Okta) rather than exposed\
  \ as an API-level OAuth flow.\n- Transport between the Python SDK and a deployed workflow is attested TLS (aTLS); the SDK only\n  submits a request if the workflow passes attestation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opaque/refs/heads/main/authentication/opaque-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- confidential-computing
- confidential-ai
- ai-governance
- data-privacy
- trusted-execution-environment
- attestation
- agentic-workflows
- retrieval-augmented-generation
- enterprise-ai
- secure-analytics
- data-clean-room
- MCP
---
