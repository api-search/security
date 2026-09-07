---
anonymous_access: false
api_key_in: []
api_specs:
- filename: authelia-api-openapi.yml
  format: yaml
  label: Authelia API
  slug: authelia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-api-openapi.yml
- filename: authelia-discovery-api-openapi.yml
  format: yaml
  label: Authelia Discovery API
  slug: authelia-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-discovery-api-openapi.yml
- filename: authelia-oidc-api-openapi.yml
  format: yaml
  label: Authelia OIDC API
  slug: authelia-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-oidc-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: 'How a caller authenticates to an Authelia deployment. Two distinct things are easy to confuse and are kept apart here: (1) authenticating TO the Authelia API, which is session-cookie based, and (2) the authentication schemes Authelia accepts at its PROXY AUTHORIZATION endpoints on behalf of the applications it protects. There is no API key issuance flow and no vendor-managed credential of any kind — Authelia is self-hosted, so all credentials belong to the operator''s deployment.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Authelia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authelia secures its APIs with apiKey and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Authelia
provider_slug: authelia
scheme_count: 2
schemes:
- applies_to: the Authelia portal API (/api/* other than /api/oidc/*)
  detail: A session cookie issued by postFirstFactor and elevated by the second-factor operations. The cookie name defaults to `authelia_session` and is configurable per deployment (session.cookies[].name), so the value declared in the contract is a default. The cookie is domain-scoped and requires https.
  in: cookie
  name: authelia_auth
  parameter: authelia_session
  sources:
  - openapi/authelia-api-openapi.yml#/components/securitySchemes/authelia_auth
  - https://www.authelia.com/configuration/session/
  type: apiKey
- applies_to: the OpenID Connect 1.0 Provider surface (/api/oidc/*)
  detail: Relying parties authenticate at the token, introspection, revocation and PAR endpoints using the client's registered token_endpoint_auth_method — client_secret_basic, client_secret_post, client_secret_jwt or private_key_jwt for confidential clients, `none` for public clients.
  name: openid
  openIdConnectUrl: <base>/.well-known/openid-configuration
  sources:
  - openapi/authelia-api-openapi.yml#/components/securitySchemes/openid
  type: openIdConnect
slug: authelia-authentication
source_filename: authelia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\ndocs: https://www.authelia.com/reference/guides/proxy-authorization/\nsource: >-\n  openapi/authelia-api-openapi.yml (first-party OpenAPI 3.2.0),\n  https://www.authelia.com/integration/openid-connect/oauth-2.0-bearer-token-usage/,\n  https://www.authelia.com/reference/guides/proxy-authorization/,\n  https://www.authelia.com/configuration/session/ and\n  https://www.authelia.com/integration/guides/securing-apps-with-basic-auth/.\ndescription: >-\n  How a caller authenticates to an Authelia deployment. Two distinct things are easy to confuse and are kept\n  apart here: (1) authenticating TO the Authelia API, which is session-cookie based, and (2) the\n  authentication schemes Authelia accepts at its PROXY AUTHORIZATION endpoints on behalf of the applications\n  it protects. There is no API key issuance flow and no vendor-managed credential of any kind — Authelia is\n  self-hosted, so all credentials belong to the operator's deployment.\n\
  summary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_program: false\n  self_service_signup: false\n  note: >-\n    Upgrades a 2026-07-11 derived profile that read a best-effort scaffold spec and reported http/basic +\n    http/bearer + an oauth2 authorizationCode flow against example.com hosts.\nschemes:\n- name: authelia_auth\n  type: apiKey\n  in: cookie\n  parameter: authelia_session\n  applies_to: the Authelia portal API (/api/* other than /api/oidc/*)\n  detail: >-\n    A session cookie issued by postFirstFactor and elevated by the second-factor operations. The cookie name\n    defaults to `authelia_session` and is configurable per deployment (session.cookies[].name), so the value\n    declared in the contract is a default. The cookie is domain-scoped and requires https.\n  sources:\n  - openapi/authelia-api-openapi.yml#/components/securitySchemes/authelia_auth\n  - https://www.authelia.com/configuration/session/\n- name: openid\n  type: openIdConnect\n  openIdConnectUrl:\
  \ <base>/.well-known/openid-configuration\n  applies_to: the OpenID Connect 1.0 Provider surface (/api/oidc/*)\n  detail: >-\n    Relying parties authenticate at the token, introspection, revocation and PAR endpoints using the\n    client's registered token_endpoint_auth_method — client_secret_basic, client_secret_post,\n    client_secret_jwt or private_key_jwt for confidential clients, `none` for public clients.\n  sources:\n  - openapi/authelia-api-openapi.yml#/components/securitySchemes/openid\nauthentication_levels:\n  description: >-\n    Authelia's authorization decisions are graded by the caller's authentication level, not by a scope.\n  levels:\n  - level: anonymous\n    meaning: No valid session.\n  - level: one_factor\n    meaning: Username and password verified (postFirstFactor) or a bearer token from the client_credentials grant.\n  - level: two_factor\n    meaning: A second factor completed — TOTP, WebAuthn/passkey or Duo push.\n  elevation: >-\n    Sensitive self-service\
  \ operations (credential management) additionally require an ELEVATED session,\n    obtained by proving control of the registered email address. See\n    https://www.authelia.com/configuration/identity-validation/elevated-session/.\nfirst_factor_methods:\n- method: password\n  backends: [file, ldap, activedirectory]\n  operation: postFirstFactor\n- method: passkey\n  detail: WebAuthn passkey login as a first factor, when enabled.\n  operation: postFirstFactorPasskey\nsecond_factor_methods:\n- method: totp\n  standard: RFC 6238\n  operations: [getSecondFactorTOTPConfiguration, postSecondFactorTOTP, postSecondFactorTOTPRegistration, deleteSecondFactorTOTP]\n- method: webauthn\n  standard: W3C WebAuthn / FIDO2\n  operations: [getSecondFactorWebAuthn, postSecondFactorWebAuthn, getSecondFactorWebAuthnCredentials, deleteSecondFactorWebAuthnCredential]\n- method: duo\n  detail: Duo Push via the Duo API.\n  operations: [getSecondFactorDuo, postSecondFactorDuo, getSecondFactorDuoDevices, postSecondFactorDuoDevice]\n\
  - method: password\n  detail: Password re-entry as a second factor when the first factor was a passkey.\n  operations: [postSecondFactorPassword]\nproxy_authorization_schemes:\n  description: >-\n    Schemes Authelia accepts at /api/authz/* on behalf of protected applications. Each is opt-in per authz\n    endpoint via server.endpoints.authz.<name>.authn_strategies.\n  strategies:\n  - name: CookieSession\n    scheme: cookie\n    default: true\n  - name: HeaderAuthorization\n    schemes: [Basic, Bearer]\n    default: false\n  - name: HeaderProxyAuthorization\n    schemes: [Basic, Bearer]\n    default: false\n  - name: HeaderAuthRequestProxyAuthorization\n    schemes: [Basic, Bearer]\n    default: false\n  - name: HeaderLegacy\n    default: true\n    note: Legacy /api/verify endpoint only.\n  basic_auth: >-\n    Basic credentials are validated against the configured authentication backend and are treated as a\n    1FA authorization. Documented as the service-account pattern for API access\
  \ at\n    https://www.authelia.com/integration/guides/securing-apps-with-basic-auth/.\n  bearer_auth:\n    scope: authelia.bearer.authz\n    token_prefixes:\n      access_token: authelia_at_\n      refresh_token: authelia_rt_\n      authorization_code: authelia_ac_\n    detail: >-\n      Only a genuine access token (authelia_at_ prefix) is accepted; refresh tokens and authorization codes\n      are rejected. The token's audience must exactly match or prefix the requested URL. A token issued via\n      client_credentials is always treated as 1FA and matches access control rules through the special\n      subject oauth2:client:<id>.\n    docs: https://www.authelia.com/integration/openid-connect/oauth-2.0-bearer-token-usage/\ntransport:\n  https_required: true\n  detail: Authelia MUST be served over https; this is a stated design decision, not a recommendation.\ngaps:\n- No API key or personal access token concept exists for the Authelia API itself.\n- Authelia's own documentation states\
  \ that authelia.bearer.authz tokens are not intended for calling the\n  Authelia API; a dedicated scope and audience scheme for that is deferred to a future release.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/authentication/authelia-authentication.yml
summary_line: apiKey/openIdConnect · 2 schemes
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open-Source
- OpenID Connect
- Self-Hosted
- SSO
---
