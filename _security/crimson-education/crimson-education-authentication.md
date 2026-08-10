---
api_key_in:
- header
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crimson Education Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Crimson Education secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Crimson Education
provider_slug: crimson-education
scheme_count: 3
schemes:
- audience: Embedded iframe sub-apps whose parent injects the JWT over postMessage, and any frontend or backend already holding a token the Crimson backend accepts.
  bearerFormat: JWT
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  notes: The SDK strips a leading "Bearer " from whatever getToken() returns before concatenating. In embedded contexts the React layer (<CrimsonProvider>) reads the token from xprops/localStorage automatically, so getToken is not hand-written.
  scheme: bearer
  sdk_config: getToken
  status: available
  token_issuer: Auth0 (Crimson Auth0 JWT)
  type: http
- audience: trusted server-to-server backends with no end-user login
  auth_scheme: crimsonauthkey
  guardrails:
  - SDK throws if serviceKey is used in a browser environment
  - SDK throws if serviceKey is empty
  - tenantDomain is effectively required; requests without it fall back to the default "crimsonapp" tenant with a warning, and package-item list calls 400
  - provider documents the key as god-mode, backend-only, never in frontend code or source control, and to be rotated
  header: 'Authorization: crimsonauthkey <key>'
  in: header
  name: serviceKey
  parameter_name: Authorization
  privilege: Service-level credential. The SDK README states that a key matching the backend CRIMSON_APP_ACCESS_KEYS allowlist is treated as isServer and BYPASSES per-user RBAC; data scope is then determined by the x-tenant-domain header plus any explicitly passed userId.
  sdk_config: serviceKey
  status: available
  type: apiKey
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    pkce: true
    scopes:
    - description: Documented in the SDK example scope array; no published scope reference exists.
      scope: profile
    tokenUrl: /oauth/token
  name: oauth2
  notes: The SDK implements authorize(), handleOAuthCallback({code,state}), token refresh, isAuthenticated() and logout(), but the README states explicitly that the backend /oauth/authorize and /oauth/token endpoints are NOT yet deployed and the mode is therefore unusable. Recorded as declared-but-unavailable, not as a live OAuth surface.
  sdk_config: oauth
  status: not-deployed
  type: oauth2
slug: crimson-education-authentication
source_filename: crimson-education-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://www.npmjs.com/package/@crimson-education/sdk\ndocs: https://www.npmjs.com/package/@crimson-education/sdk\nnotes: >-\n  Crimson Education publishes no OpenAPI and no developer-portal auth page, so this\n  profile is read from the first-party SDK @crimson-education/sdk (v0.3.38), whose\n  README documents three mutually exclusive authentication modes on CrimsonClient.\n  The SDK is the provider's own published artifact; nothing here is inferred beyond\n  what it states.\nsummary:\n  types: [http, apiKey, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  oauth2_status: not-deployed\n  mutually_exclusive: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer <token>'\n  sdk_config: getToken\n  status: available\n  token_issuer: Auth0 (Crimson Auth0 JWT)\n  audience: >-\n    Embedded iframe sub-apps whose parent\
  \ injects the JWT over postMessage, and any\n    frontend or backend already holding a token the Crimson backend accepts.\n  notes: >-\n    The SDK strips a leading \"Bearer \" from whatever getToken() returns before\n    concatenating. In embedded contexts the React layer (<CrimsonProvider>) reads the\n    token from xprops/localStorage automatically, so getToken is not hand-written.\n- name: serviceKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  header: 'Authorization: crimsonauthkey <key>'\n  auth_scheme: crimsonauthkey\n  sdk_config: serviceKey\n  status: available\n  audience: trusted server-to-server backends with no end-user login\n  privilege: >-\n    Service-level credential. The SDK README states that a key matching the backend\n    CRIMSON_APP_ACCESS_KEYS allowlist is treated as isServer and BYPASSES per-user\n    RBAC; data scope is then determined by the x-tenant-domain header plus any\n    explicitly passed userId.\n  guardrails:\n  - SDK throws if serviceKey\
  \ is used in a browser environment\n  - SDK throws if serviceKey is empty\n  - tenantDomain is effectively required; requests without it fall back to the default\n    \"crimsonapp\" tenant with a warning, and package-item list calls 400\n  - provider documents the key as god-mode, backend-only, never in frontend code or\n    source control, and to be rotated\n- name: oauth2\n  type: oauth2\n  sdk_config: oauth\n  status: not-deployed\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes:\n    - scope: profile\n      description: 'Documented in the SDK example scope array; no published scope reference exists.'\n  notes: >-\n    The SDK implements authorize(), handleOAuthCallback({code,state}), token refresh,\n    isAuthenticated() and logout(), but the README states explicitly that the backend\n    /oauth/authorize and /oauth/token endpoints are NOT yet deployed and the mode is\n    therefore unusable. Recorded\
  \ as declared-but-unavailable, not as a live OAuth\n    surface.\ntenancy:\n  header: x-tenant-domain\n  sdk_config: tenantDomain\n  default: crimsonapp\n  required_for: service-key mode\n  example_value: app.crimsoneducation.org\n  notes: >-\n    In bearer mode the tenant is resolved from the user; in service-key mode there is\n    no end user, so the tenant must be named explicitly.\nidentity_endpoints:\n- {path: /api/v1/account/me/profile, returns: 'userId, email, firstName, lastName, nickname, name, picture, status, isMultiTenant, roles[], tenant'}\n- {path: /api/v1/account/me/roles, returns: 'userId, roles[{roleId,isPrimary}]'}\n- {path: /api/v1/account/linked-tenants, returns: linked tenant accounts for multi-tenant users}\n- {path: /api/v1/indigo/me, returns: 'Indigo identity: role student|tutor, tenantId, tenantName, isMultiTenant, relatedAccounts[]', requires: INDIGO product subscription}\ndiscovery:\n  openid_configuration: absent (404 on both API hosts)\n  oauth_authorization_server:\
  \ absent (404 on both API hosts)\n  oauth_protected_resource: absent (404 on both API hosts)\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://registry.npmjs.org/@crimson-education%2Fsdk\n  http_status: 200\n  package_version: 0.3.38\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crimson-education/refs/heads/main/authentication/crimson-education-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- Education
- EdTech
- Admissions
- Tutoring
- Students
- Online Learning
- Mentoring
---
