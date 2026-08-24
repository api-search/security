---
api_key_in: []
auth_types: []
description: Authentication profile for the INK Games API surface. INK Games publishes no developer authentication documentation of any kind — there is no developer portal, no API key issuance flow, and no OAuth or OIDC discovery document on any host (see well-known/ink-games-well-known.yml). Everything below is derived from the GraphQL schema retrieved by anonymous introspection and from the responses the live hosts actually returned.
kind: authentication
layout: security
method: derived
name: Ink Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: INK Games declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: INK Games
provider_slug: ink-games
scheme_count: 2
schemes:
- bearerFormat: JWT
  documented_by_provider: false
  evidence: 'The schema exposes the Strapi users-permissions plugin: mutation login(input: UsersPermissionsLoginInput!): UsersPermissionsLoginPayload! returning a `jwt` String and a `user` UsersPermissionsMe, plus register, forgotPassword, resetPassword, changePassword and emailConfirmation. UsersPermissionsLoginInput takes identifier/password/provider, so the credential is an identifier+password exchanged for a JWT presented as `Authorization: Bearer <jwt>`.'
  id: strapi-users-permissions-jwt
  method: derived
  note: Strapi's users-permissions plugin also accepts a long-lived API token as a bearer credential on the same header. Which credential class INK Games actually issues is not observable anonymously.
  scheme: bearer
  source: graphql/ink-games-cms-schema.graphql
  surface: https://webadm.inkgames.com/graphql
  type: http
- documented_by_provider: false
  evidence: Every path probed returned HTTP 403 {"message":"Missing Authentication Token"}, which is AWS API Gateway's standard response for a route that does not exist on the deployed API, not an authentication challenge. No WWW-Authenticate header, no OAuth metadata document, no error body naming a scheme.
  id: aws-api-gateway-unknown
  method: probed
  note: The dashboard bundle at https://dashboard.inkgames.com/assets/index-18895c2e.js calls https://ip-api.inkgames.com/user/validate-auth-code, and the shell loads simplewebauthn (/vendors/simplewebauthn/index.es5.umd.min.js), so the consumer login flow involves an emailed/SMS auth code plus WebAuthn passkeys. The wire credential for the API itself is not published and was not observed.
  source: HTTP probe 2026-08-23
  surface: https://ip-api.inkgames.com
  type: unknown
slug: ink-games-authentication
source_filename: ink-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: graphql/ink-games-cms-schema.graphql + live probes of every INK Games API host\ndescription: >-\n  Authentication profile for the INK Games API surface. INK Games publishes no\n  developer authentication documentation of any kind — there is no developer portal,\n  no API key issuance flow, and no OAuth or OIDC discovery document on any host (see\n  well-known/ink-games-well-known.yml). Everything below is derived from the GraphQL\n  schema retrieved by anonymous introspection and from the responses the live hosts\n  actually returned.\n\nschemes:\n  - id: strapi-users-permissions-jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    surface: https://webadm.inkgames.com/graphql\n    method: derived\n    source: graphql/ink-games-cms-schema.graphql\n    evidence: >-\n      The schema exposes the Strapi users-permissions plugin: mutation login(input:\n      UsersPermissionsLoginInput!): UsersPermissionsLoginPayload!\
  \ returning a `jwt`\n      String and a `user` UsersPermissionsMe, plus register, forgotPassword,\n      resetPassword, changePassword and emailConfirmation. UsersPermissionsLoginInput\n      takes identifier/password/provider, so the credential is an identifier+password\n      exchanged for a JWT presented as `Authorization: Bearer <jwt>`.\n    documented_by_provider: false\n    note: >-\n      Strapi's users-permissions plugin also accepts a long-lived API token as a\n      bearer credential on the same header. Which credential class INK Games actually\n      issues is not observable anonymously.\n\n  - id: aws-api-gateway-unknown\n    type: unknown\n    surface: https://ip-api.inkgames.com\n    method: probed\n    source: 'HTTP probe 2026-08-23'\n    evidence: >-\n      Every path probed returned HTTP 403 {\"message\":\"Missing Authentication Token\"},\n      which is AWS API Gateway's standard response for a route that does not exist on\n      the deployed API, not an authentication\
  \ challenge. No WWW-Authenticate header,\n      no OAuth metadata document, no error body naming a scheme.\n    documented_by_provider: false\n    note: >-\n      The dashboard bundle at https://dashboard.inkgames.com/assets/index-18895c2e.js\n      calls https://ip-api.inkgames.com/user/validate-auth-code, and the shell loads\n      simplewebauthn (/vendors/simplewebauthn/index.es5.umd.min.js), so the consumer\n      login flow involves an emailed/SMS auth code plus WebAuthn passkeys. The wire\n      credential for the API itself is not published and was not observed.\n\nanonymous_access:\n  graphql_introspection: allowed\n  graphql_resolvers: denied\n  note: >-\n    Anonymous callers can read the complete GraphQL type system but every resolver\n    returns {\"errors\":[{\"message\":\"Forbidden access\",\"extensions\":{\"code\":\"FORBIDDEN\"}}]}.\n    The Strapi Public role has no content permissions granted.\n\nnot_present:\n  oauth2: >-\n    No oauth2 securityScheme, no /.well-known/oauth-authorization-server\
  \ on any host,\n    no documented authorization or token endpoint. No scopes artifact is derivable.\n  openid_connect: No /.well-known/openid-configuration on any host (all probes 404 or soft-404).\n  mtls: Not offered or documented.\n  api_key_program: No public key issuance, no developer account, no key-prefix convention published.\n\nobservations:\n  - id: cors-wildcard-with-credentials\n    severity: informational\n    surface: https://webadm.inkgames.com/graphql\n    finding: >-\n      The endpoint returns `access-control-allow-origin: *` together with\n      `access-control-allow-credentials: true` on an anonymous request. Browsers\n      reject that combination, so it is a misconfiguration rather than an exposure,\n      but it is the deployed header set.\n    evidence: 'observed response headers, POST https://webadm.inkgames.com/graphql, HTTP 200, 2026-08-23'\n  - id: stack-traces-in-errors\n    severity: informational\n    surface: https://webadm.inkgames.com/graphql\n    finding:\
  \ >-\n      Anonymous FORBIDDEN responses include a full `extensions.stacktrace` array\n      disclosing absolute server filesystem paths (/home/ubuntu/strapi/ink-web/...)\n      and the Strapi plugin version layout. Strapi suppresses this when NODE_ENV is\n      production.\n    evidence: 'observed response body, POST https://webadm.inkgames.com/graphql, HTTP 200, 2026-08-23'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ink-games/refs/heads/main/authentication/ink-games-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Games
- Gaming
- Mobile Games
- Entertainment
- Consumer
- Rewards
- Payments
- Loyalty
- Referral
- GraphQL
- Content Management
---
