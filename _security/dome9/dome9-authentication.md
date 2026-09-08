---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dome9-api-openapi.json
  format: json
  label: Dome9 API
  slug: dome9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dome9/refs/heads/main/openapi/dome9-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dome9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dome9 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dome9
provider_slug: dome9
scheme_count: 1
schemes:
- credential_issuance:
    console: https://secure.dome9.com
    docs: https://sc1.checkpoint.com/documents/CloudGuard_Dome9/Documentation/Settings/Credentials.htm
    where: CloudGuard web application, Settings > Credentials
  description: HTTP Basic authentication. The username is the V2 API key id and the password is the API key secret.
  example: curl -u your-api-key-id:your-api-key-secret https://api.dome9.com/v2/CloudAccounts
  name: API key V2
  scheme: basic
  sources:
  - openapi/dome9-api-openapi.json
  - https://docs.cgn.portal.checkpoint.com/reference/authentication
  spec_name_note: 'The contract calls this securityDefinition "API key V2" but declares `type: basic` — it is HTTP Basic carrying an API key pair, not an apiKey-in-header scheme.'
  type: http
slug: dome9-authentication
source_filename: dome9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://docs.cgn.portal.checkpoint.com/reference/authentication (fetched\n  2026-09-07) plus openapi/dome9-api-openapi.json, the first-party Swagger 2.0\n  contract at https://api.dome9.com/swagger/docs/v2.\ndocs: https://docs.cgn.portal.checkpoint.com/reference/authentication\nprovider: Dome9\nproviderId: dome9\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_key_header: false\nschemes:\n- name: API key V2\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The username is the V2 API key id and the\n    password is the API key secret.\n  spec_name_note: >-\n    The contract calls this securityDefinition \"API key V2\" but declares\n    `type: basic` — it is HTTP Basic carrying an API key pair, not an\n    apiKey-in-header scheme.\n  credential_issuance:\n    where: CloudGuard web application, Settings > Credentials\n    console: https://secure.dome9.com\n\
  \    docs: https://sc1.checkpoint.com/documents/CloudGuard_Dome9/Documentation/Settings/Credentials.htm\n  example: curl -u your-api-key-id:your-api-key-secret https://api.dome9.com/v2/CloudAccounts\n  sources:\n  - openapi/dome9-api-openapi.json\n  - https://docs.cgn.portal.checkpoint.com/reference/authentication\nauthorization_model:\n  style: inherited-user-permissions\n  scopes: false\n  detail: >-\n    Quoting the docs: \"Your permissions when using the REST API with the key will\n    be the same as the permissions of the CloudGuard user who generated the key\n    from the CloudGuard web application.\" There is no scope, audience or\n    least-privilege narrowing at the key level — the blast radius of a key is the\n    blast radius of its creator. Narrowing is done by creating the key under a\n    purpose-built user with a restricted Role (/v2/Role) or a ServiceAccount\n    (/v2/serviceaccount).\n  rbac_surface:\n  - /v2/Role\n  - /v2/user\n  - /v2/serviceaccount\n  - /v2/account/sso\n\
  other_credentials:\n- name: assume-role JWT\n  path: /v2/auth/assume-role/jwt\n  purpose: >-\n    Used by the CloudGuard image-scan CI/CD tooling to exchange for a\n    short-lived token. Documented in the connectivity endpoint tables, not as a\n    general-purpose auth flow, and it is not an OAuth authorization server.\ngaps:\n- No OAuth 2.0 or OpenID Connect.\n- No scopes; see the absence of scopes/dome9-scopes.yml in this repo.\n- No key rotation or expiry policy published.\n- No mTLS.\n- No /.well-known/openid-configuration or oauth-authorization-server on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dome9/refs/heads/main/authentication/dome9-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Compliance
- Infrastructure Security
- Multi-Cloud
- Security Posture Management
---
