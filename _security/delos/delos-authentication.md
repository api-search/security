---
api_key_in:
- header
api_specs:
- filename: delos-wellcube-cloud-be-openapi.yml
  format: yaml
  label: WellCube Cloud BE API
  slug: wellcube-cloud-be-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-wellcube-cloud-be-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Delos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delos secures its APIs with apiKey and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delos
provider_slug: delos
scheme_count: 1
schemes:
- applied: global
  in: header
  name: Authorization
  operations: 39
  parameter: Authorization
  sources:
  - openapi/delos-wellcube-cloud-be-openapi.yml
  type: apiKey
slug: delos-authentication
source_filename: delos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/delos-wellcube-cloud-be-openapi.yml\ndocs: https://cloud.wellcube.io/api/v1/docs/\nevidence:\n- https://cloud.wellcube.io/api/v1/docs/\n- https://app.wellcube.io/config.js\n- https://cognito-idp.us-east-1.amazonaws.com/us-east-1_QNxQ6AqaQ/.well-known/openid-configuration\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The OpenAPI declares exactly one security scheme — an apiKey named `Authorization` carried in the\n    request header — and applies it globally via a root-level `security` requirement, so all 39\n    operations are authenticated. The scheme is declared as `apiKey` rather than\n    `http`/`bearer`, which is a spec-modelling choice, not a second mechanism: the value is the JWT\n    the API itself mints. Two token-issuing paths exist in the same spec, and a third, federated path\n    is visible in the app's public runtime config.\nschemes:\n\
  - name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  applied: global\n  operations: 39\n  sources:\n  - openapi/delos-wellcube-cloud-be-openapi.yml\ntoken_issuance:\n- flow: password\n  name: Full session\n  operation: sessionCreate\n  endpoint: POST https://cloud.wellcube.io/api/v1/sessions\n  credentials: [email, password, product]\n  returns: jwt\n  note: >-\n    The spec's own response description for this operation reads \"Deprecated create session response\"\n    — the provider is signalling that the response envelope of its primary login operation is\n    deprecated, while shipping no replacement operation and no deprecation date. See\n    lifecycle/delos-lifecycle.yml.\n- flow: password-limited\n  name: Limited session\n  operation: limitedSessionCreate\n  endpoint: POST https://cloud.wellcube.io/api/v1/limited-sessions\n  returns: {accessToken: string, refreshToken: string}\n  schema: AccessData\n  refresh_operation: limitedSessionRefresh\n  refresh_endpoint:\
  \ POST https://cloud.wellcube.io/api/v1/limited-sessions/refresh\n  note: >-\n    The newer of the two paths — issues a proper access/refresh pair (components.schemas.AccessData)\n    instead of a bare `jwt`, and is the only operation with an explicit refresh counterpart.\n- flow: federated\n  name: Cognito session exchange (admin)\n  operations: [adminUserCognitoSessionCreate, adminUserLimitedCognitoSessionCreate]\n  endpoints:\n  - POST https://cloud.wellcube.io/api/v1/admin/users/cognito-sessions\n  - POST https://cloud.wellcube.io/api/v1/admin/users/limited-cognito-sessions\n  note: Exchanges an AWS Cognito identity for a Cloud BE session. Admin-scoped.\nidentity_provider:\n  vendor: AWS Cognito\n  user_pool_id: us-east-1_QNxQ6AqaQ\n  region: us-east-1\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_QNxQ6AqaQ\n  discovery: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_QNxQ6AqaQ/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_QNxQ6AqaQ/.well-known/jwks.json\n\
  \  scopes_supported: [openid, email, phone, profile]\n  id_token_signing_alg_values_supported: [RS256]\n  source: >-\n    https://app.wellcube.io/config.js — the WellCube web application's public runtime configuration,\n    which names the user pool. The discovery document itself is served by AWS, not by Delos.\n  note: >-\n    The Cognito pool advertises only the four standard OIDC scopes. There is no resource server, no\n    custom scope namespace, and no scope-to-permission mapping anywhere in the OpenAPI — authorization\n    in the Cloud BE API is role/ownership-based (`x-permission-denied` appears on 28 of 39 operations)\n    rather than scope-based. That is why no scopes/ artifact is emitted for this provider.\ngaps:\n- The OpenAPI never documents the token format, lifetime, or refresh semantics of the `Authorization` header value.\n- No `bearerFormat`, no `description` on the security scheme.\n- Local-account operations accept installation credentials (localAccountLink/Share/Transfer\
  \ return\n  `x-wrong-credentials`), a second credential domain the spec does not describe.\n- No published rotation, revocation, or key-management policy for API consumers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/authentication/delos-authentication.yml
summary_line: apiKey/openIdConnect · 1 scheme
tags:
- wellness-real-estate
- Indoor Air Quality
- indoor-environmental-quality
- IoT
- Smart Buildings
- Building Automation
- Air Purification
- environmental-sensors
- Commercial Real Estate
- healthy-buildings
- Hospitality
- ESG
---
