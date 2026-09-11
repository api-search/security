---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fermyon-accounts-api-openapi.yml
  format: yaml
  label: Fermyon accounts API
  slug: fermyon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-accounts-api-openapi.yml
- filename: fermyon-apps-api-openapi.yml
  format: yaml
  label: Fermyon apps API
  slug: fermyon-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-apps-api-openapi.yml
- filename: fermyon-auth-tokens-api-openapi.yml
  format: yaml
  label: Fermyon auth-tokens API
  slug: fermyon-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-auth-tokens-api-openapi.yml
- filename: fermyon-channels-api-openapi.yml
  format: yaml
  label: Fermyon channels API
  slug: fermyon-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-channels-api-openapi.yml
- filename: fermyon-custom-domains-api-openapi.yml
  format: yaml
  label: Fermyon custom-domains API
  slug: fermyon-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-custom-domains-api-openapi.yml
- filename: fermyon-device-codes-api-openapi.yml
  format: yaml
  label: Fermyon device-codes API
  slug: fermyon-device-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-device-codes-api-openapi.yml
- filename: fermyon-key-value-pairs-api-openapi.yml
  format: yaml
  label: Fermyon key-value-pairs API
  slug: fermyon-key-value-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-pairs-api-openapi.yml
- filename: fermyon-key-value-stores-api-openapi.yml
  format: yaml
  label: Fermyon key-value-stores API
  slug: fermyon-key-value-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-stores-api-openapi.yml
- filename: fermyon-oci-api-openapi.yml
  format: yaml
  label: Fermyon oci API
  slug: fermyon-oci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-oci-api-openapi.yml
- filename: fermyon-payments-api-openapi.yml
  format: yaml
  label: Fermyon payments API
  slug: fermyon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-payments-api-openapi.yml
- filename: fermyon-personal-access-tokens-api-openapi.yml
  format: yaml
  label: Fermyon personal-access-tokens API
  slug: fermyon-personal-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-personal-access-tokens-api-openapi.yml
- filename: fermyon-revisions-api-openapi.yml
  format: yaml
  label: Fermyon revisions API
  slug: fermyon-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-revisions-api-openapi.yml
- filename: fermyon-sql-databases-api-openapi.yml
  format: yaml
  label: Fermyon sql-databases API
  slug: fermyon-sql-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-sql-databases-api-openapi.yml
- filename: fermyon-variable-pairs-api-openapi.yml
  format: yaml
  label: Fermyon variable-pairs API
  slug: fermyon-variable-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-variable-pairs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fermyon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fermyon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fermyon
provider_slug: fermyon
scheme_count: 1
schemes:
- description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/fermyon-accounts-api-openapi.yml
  - openapi/fermyon-apps-api-openapi.yml
  - openapi/fermyon-auth-tokens-api-openapi.yml
  - openapi/fermyon-channels-api-openapi.yml
  - openapi/fermyon-custom-domains-api-openapi.yml
  - openapi/fermyon-device-codes-api-openapi.yml
  - openapi/fermyon-key-value-pairs-api-openapi.yml
  - openapi/fermyon-key-value-stores-api-openapi.yml
  - openapi/fermyon-oci-api-openapi.yml
  - openapi/fermyon-payments-api-openapi.yml
  - openapi/fermyon-personal-access-tokens-api-openapi.yml
  - openapi/fermyon-revisions-api-openapi.yml
  - openapi/fermyon-sql-databases-api-openapi.yml
  - openapi/fermyon-variable-pairs-api-openapi.yml
  type: apiKey
slug: fermyon-authentication
source_filename: fermyon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/fermyon-accounts-api-openapi.yml, openapi/fermyon-apps-api-openapi.yml, openapi/fermyon-auth-tokens-api-openapi.yml,\n  openapi/fermyon-channels-api-openapi.yml, openapi/fermyon-custom-domains-api-openapi.yml, openapi/fermyon-device-codes-api-openapi.yml,\n  openapi/fermyon-key-value-pairs-api-openapi.yml, openapi/fermyon-key-value-stores-api-openapi.yml, openapi/fermyon-oci-api-openapi.yml,\n  openapi/fermyon-payments-api-openapi.yml, openapi/fermyon-personal-access-tokens-api-openapi.yml, openapi/fermyon-revisions-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer {token}\"'\n  sources:\n  - openapi/fermyon-accounts-api-openapi.yml\n  - openapi/fermyon-apps-api-openapi.yml\n  - openapi/fermyon-auth-tokens-api-openapi.yml\n\
  \  - openapi/fermyon-channels-api-openapi.yml\n  - openapi/fermyon-custom-domains-api-openapi.yml\n  - openapi/fermyon-device-codes-api-openapi.yml\n  - openapi/fermyon-key-value-pairs-api-openapi.yml\n  - openapi/fermyon-key-value-stores-api-openapi.yml\n  - openapi/fermyon-oci-api-openapi.yml\n  - openapi/fermyon-payments-api-openapi.yml\n  - openapi/fermyon-personal-access-tokens-api-openapi.yml\n  - openapi/fermyon-revisions-api-openapi.yml\n  - openapi/fermyon-sql-databases-api-openapi.yml\n  - openapi/fermyon-variable-pairs-api-openapi.yml\ndocs:\n- https://developer.fermyon.com/cloud/user-settings\n- https://developer.fermyon.com/cloud/cloud-command-reference\n- https://techdocs.akamai.com/akamai-functions/docs/manage-accounts\nnote: 'Upgraded from derived to searched on 2026-09-09 against the Fermyon Cloud documentation. The single\n  Bearer scheme below is the whole story: a JWT in the Authorization header on all 61 operations, no scopes,\n  no oauth2 securityScheme, and no OpenID\
  \ metadata. Token acquisition is not in the securityScheme but\n  is fully specified by the contract, so it is recorded here.'\ntoken_acquisition:\n- method: personal-access-token\n  operations:\n  - POST /api/personal-access-tokens\n  - GET /api/personal-access-tokens\n  - DELETE /api/personal-access-tokens/{id}\n  note: The token value is returned once, in PersonalAccessTokenValue. Listing returns only id, name and\n    createdAt.\n- method: device-code\n  operations:\n  - POST /api/device-codes\n  - GET /api/device-codes/{userCode}\n  - POST /api/device-codes/activate\n  note: What `spin cloud login` drives. DeviceCodeItem returns deviceCode, userCode, verificationUrl,\n    expiresIn and interval — the RFC 8628 device authorization response fields, camelCased — but the endpoints\n    and token exchange are not RFC 8628. See conformance/fermyon-conformance.yml.\n- method: token-exchange-and-refresh\n  operations:\n  - POST /api/auth-tokens\n  - POST /api/auth-tokens/refresh\n  note:\
  \ Returns TokenInfo {token, refreshToken, expiration}.\nauthorization:\n  scopes: []\n  rbac: false\n  evidence: 'No scopes are declared anywhere in the contract and no permission or role entity exists in\n    any schema. The Akamai Functions documentation states it outright: \"Akamai Functions does not support\n    Role-Based Access Control (RBAC). Everyone has the same level of permissions and any member can permanently\n    delete any application in the account.\" (https://techdocs.akamai.com/akamai-functions/docs/manage-accounts)'\n  agent_impact: A token cannot be scoped down. Any token an agent holds can delete every application in\n    the account.\ncredential_storage:\n  cli: As of `spin aka` v0.7.0 (2026-03-20) plugin login credentials are stored in the operating system\n    native secret store — macOS Keychain, Linux secret service, Windows Credential Manager — rather than\n    a plain-text config file. Existing credentials migrate automatically. (https://techdocs.akamai.com/akamai-functions/changelog/mar-20-2026-spin-aka-v070-updates)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/authentication/fermyon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Functions
- WebAssembly
- Serverless
- Edge Computing
- Serverless Functions
- Spin
- Developer Tools
---
