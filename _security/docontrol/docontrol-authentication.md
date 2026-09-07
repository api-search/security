---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docontrol-authentication-api-openapi.yml
  format: yaml
  label: DoControl Authentication API
  slug: docontrol-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-authentication-api-openapi.yml
- filename: docontrol-graphql-api-openapi.yml
  format: yaml
  label: DoControl GraphQL API
  slug: docontrol-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-graphql-api-openapi.yml
auth_types:
- http
- apiKey
description: Two-step credential flow. A long-lived API key (which DoControl calls a refresh token) is minted in the console and exchanged at a bespoke endpoint for a five-minute bearer access token, which is then presented to the GraphQL gateway. This is NOT OAuth 2.0 — there is no grant_type, no client identity, no scope parameter and no authorization-server metadata document.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Docontrol Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoControl secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DoControl
provider_slug: docontrol
scheme_count: 2
schemes:
- applies_to:
  - https://apollo-gateway-v4-api.prod.docontrol.io/graphql
  description: Access token returned from the token exchange; valid for 5 minutes.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/docontrol-authentication-api-openapi.yml
  - openapi/docontrol-graphql-api-openapi.yml
  type: http
- applies_to:
  - https://auth.prod.docontrol.io/refresh
  description: 'The API key created in the DoControl admin panel, presented in the JSON body of the token exchange. Valid for 10 years. Not modelled as a securityScheme in the spec (the /refresh operation is declared `security: []`), but it is the credential that actually gates the API.'
  field: refreshToken
  in: body
  name: refreshToken
  source: https://docs.docontrol.io/docontrol-user-guide/system-management/settings/api-keys.md
  type: apiKey
slug: docontrol-authentication
source_filename: docontrol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://docs.docontrol.io/docontrol-user-guide/system-management/api.md and\n  https://docs.docontrol.io/docontrol-user-guide/system-management/settings/api-keys.md, joined to\n  the securitySchemes in openapi/docontrol-authentication-api-openapi.yml and\n  openapi/docontrol-graphql-api-openapi.yml. Live behaviour probed 2026-09-06.\nprovider: DoControl\nproviderId: docontrol\ndocs: https://docs.docontrol.io/docontrol-user-guide/system-management/api.md\ndescription: >-\n  Two-step credential flow. A long-lived API key (which DoControl calls a refresh token) is minted\n  in the console and exchanged at a bespoke endpoint for a five-minute bearer access token, which\n  is then presented to the GraphQL gateway. This is NOT OAuth 2.0 — there is no grant_type, no\n  client identity, no scope parameter and no authorization-server metadata document.\nsummary:\n  types:\n  - http\n  - apiKey\n  oauth2: false\n  oidc: false\n\
  \  mtls: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token returned from the token exchange; valid for 5 minutes.\n  in: header\n  header: Authorization\n  applies_to:\n  - https://apollo-gateway-v4-api.prod.docontrol.io/graphql\n  sources:\n  - openapi/docontrol-authentication-api-openapi.yml\n  - openapi/docontrol-graphql-api-openapi.yml\n- name: refreshToken\n  type: apiKey\n  in: body\n  field: refreshToken\n  description: >-\n    The API key created in the DoControl admin panel, presented in the JSON body of the token\n    exchange. Valid for 10 years. Not modelled as a securityScheme in the spec (the /refresh\n    operation is declared `security: []`), but it is the credential that actually gates the API.\n  applies_to:\n  - https://auth.prod.docontrol.io/refresh\n  source: https://docs.docontrol.io/docontrol-user-guide/system-management/settings/api-keys.md\nflow:\n- step: 1\n  action: Create an API key\n  where: DoControl console —\
  \ Settings > Admin > API keys\n  yields: refresh token (shown once, unrecoverable afterwards)\n  requires: admin or super-admin console permission\n- step: 2\n  action: Exchange the refresh token for an access token\n  request: 'POST https://auth.prod.docontrol.io/refresh  {\"refreshToken\": \"<api key>\"}'\n  yields: '{\"token\": \"<access token>\", \"expiresIn\": 300, \"refreshToken\": \"<refresh token>\"}'\n  note: >-\n    The response field carrying the short-lived credential is `token`, not `accessToken`. The\n    harvested OpenAPI models it as `accessToken`; DoControl's own MCP server README documents\n    `token` and warns explicitly not to confuse it with `refreshToken`. Corrected in\n    overlays/docontrol-authentication-api-overlay.yaml.\n  source: https://github.com/docontrol-io/dc-mcp-server\n- step: 3\n  action: Call the GraphQL gateway\n  request: 'POST https://apollo-gateway-v4-api.prod.docontrol.io/graphql  Authorization: Bearer <token>'\n  requires: at least admin permission\
  \ on the key\nprivilege_levels:\n- name: super-admin\n  description: Can change any functionality including system configuration and Team settings.\n- name: admin\n  description: Can change any functionality including system configuration, but not Team settings.\n- name: viewer\n  description: Read-only; cannot read anything under Settings, and cannot access the API keys tab.\n- note: >-\n    An admin can mint admin and viewer keys but not super-admin keys; only a super-admin can mint a\n    super-admin key. These are console privilege levels attached to a key, not OAuth scopes — a\n    caller cannot request a narrower grant at exchange time, and there is no scope parameter or\n    downscoping mechanism.\ncredential_hygiene:\n  max_keys_per_tenant: 10\n  key_name_charset: '[a-zA-Z0-9_]'\n  key_names_unique: true\n  refresh_token_ttl: 10 years\n  access_token_ttl_seconds: 300\n  rotation_policy_published: false\n  revocation: Delete the key in Settings > Admin > API keys.\n  risk_note:\
  \ >-\n    A 10-year bearer-equivalent credential with no published rotation guidance and no per-key\n    scoping beyond three coarse levels is the weakest part of this auth model. The minimum useful\n    key for API access is `admin`, which is also a key that can change system configuration —\n    least privilege is not reachable for a read-only integration that needs anything under\n    Settings.\nobserved:\n- url: https://apollo-gateway-v4-api.prod.docontrol.io/graphql\n  request: POST with no Authorization header\n  status: 401\n  body: MISSING ACCESS_TOKEN\n  observed: '2026-09-06'\n- url: https://auth.prod.docontrol.io/refresh\n  request: 'POST {\"refreshToken\":\"invalid\"}'\n  status: 400\n  body: (empty)\n  observed: '2026-09-06'\ndiscovery_documents:\n  oauth_authorization_server: 404 on every host\n  openid_configuration: 404 on every host\n  oauth_protected_resource: 404 on every host\n  cross_link: well-known/docontrol-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/authentication/docontrol-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Data Security
- SaaS Security
- Data Access Governance
- Data Loss Prevention
- Insider Risk Management
- SSPM
- GraphQL
- MCP
---
