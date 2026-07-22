---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: RightRev's REST and GraphQL APIs are protected by OAuth 2.0 / OpenID Connect, issued by a Keycloak identity server per tenant. Clients exchange credentials for a short-lived JWT bearer access token and present it in the Authorization header. Credentials (client_id / client_secret / username / password) are provisioned per tenant during onboarding via a support ticket.
kind: authentication
layout: security
method: searched
name: Rightrev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rightrev secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rightrev
provider_slug: rightrev
scheme_count: 3
schemes:
- description: Resource Owner Password Credentials grant for trusted clients. POST client_id, client_secret, grant_type=password, username and password (application/x-www-form-urlencoded) to the tenant realm token endpoint.
  flow: password
  grant_type: password
  name: oauth2Password
  scopes:
  - profile
  - email
  tokenUrl: https://auth.rightrev.cloud/auth/realms/<tenant_id>/protocol/openid-connect/token
  type: oauth2
- description: Implicit flow — the client retrieves an access token via the browser using the client_id, for browser-based / less-trusted clients.
  flow: implicit
  name: oauth2Implicit
  type: oauth2
- bearerFormat: JWT
  description: 'The access_token returned by the token endpoint is presented as ''Authorization: Bearer <access_token>'' on every API request. Access tokens are JWTs that expire after 300 seconds; refresh tokens last 1800 seconds.'
  name: bearerToken
  scheme: bearer
  type: http
slug: rightrev-authentication
source_filename: rightrev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://apis.rightrev.com/getting-started/authentication.md,\n  https://apis.rightrev.com/getting-started/use-bearer-token-flow.md,\n  https://apis.rightrev.com/getting-started/using-implicit-or-password-flow.md\n  — RightRev publishes no OpenAPI spec, so this profile is captured from the\n  GitBook developer documentation rather than derived from securitySchemes.\ndocs: https://apis.rightrev.com/getting-started/authentication.md\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\ndescription: >-\n  RightRev's REST and GraphQL APIs are protected by OAuth 2.0 / OpenID Connect,\n  issued by a Keycloak identity server per tenant. Clients exchange credentials\n  for a short-lived JWT bearer access token and present it in the Authorization\n  header. Credentials (client_id / client_secret / username / password) are\n  provisioned per tenant during onboarding via a support ticket.\nschemes:\n- name: oauth2Password\n  type:\
  \ oauth2\n  flow: password\n  tokenUrl: https://auth.rightrev.cloud/auth/realms/<tenant_id>/protocol/openid-connect/token\n  grant_type: password\n  description: >-\n    Resource Owner Password Credentials grant for trusted clients. POST\n    client_id, client_secret, grant_type=password, username and password\n    (application/x-www-form-urlencoded) to the tenant realm token endpoint.\n  scopes:\n  - profile\n  - email\n- name: oauth2Implicit\n  type: oauth2\n  flow: implicit\n  description: >-\n    Implicit flow — the client retrieves an access token via the browser using\n    the client_id, for browser-based / less-trusted clients.\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    The access_token returned by the token endpoint is presented as\n    'Authorization: Bearer <access_token>' on every API request. Access tokens\n    are JWTs that expire after 300 seconds; refresh tokens last 1800 seconds.\ntoken:\n  token_type: bearer\n  access_token_ttl_seconds:\
  \ 300\n  refresh_token_ttl_seconds: 1800\n  identity_provider: Keycloak (per-tenant realm)\nprovisioning: >-\n  client_id, client_secret and user credentials are issued during tenant\n  onboarding via a RightRev support ticket; there is no self-service key portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightrev/refs/heads/main/authentication/rightrev-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Revenue Recognition
- Accounting
- Finance
- Billing
- ASC 606
- IFRS 15
- Revenue
- SaaS Metrics
---
