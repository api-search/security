---
api_key_in:
- header
api_specs:
- filename: 401go-openapi-original.json
  format: json
  label: 401GO API
  slug: 401go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-openapi-original.json
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 401Go Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: 401GO secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: 401GO
provider_slug: 401go
scheme_count: 3
schemes:
- access_token_lifetime_seconds: 3600
  endpoints:
    authorization: https://app.401go.com/api/o/authorize
    discovery: https://app.401go.com/api/o/.well-known/openid-configuration
    jwks: https://app.401go.com/api/o/.well-known/jwks.json
    token: https://app.401go.com/api/o/token
    userinfo: https://app.401go.com/api/o/userinfo
  flows:
  - code_challenge_methods:
    - plain
    - S256
    docs: https://developer.401go.com/docs/authentication
    exchange_parameters:
    - grant_type=authorization_code
    - code
    - redirect_uri
    - client_id
    - client_secret
    flow: authorizationCode
    note: If a user has multiple accounts (participant, company, advisor) they must select which account to grant access to before the code is issued.
    parameters:
    - response_type=code
    - client_id
    - redirect_uri
    - scope
    - state
    pkce: true
    preferred: true
  - client_auth: 'Authorization: Basic base64(client_id:client_secret)'
    content_type: application/x-www-form-urlencoded
    docs: https://developer.401go.com/docs/client-credentials-flow
    flow: clientCredentials
    note: Entities the client credentials may access are fixed during onboarding; expanding them requires a request to 401GO.
    parameters:
    - grant_type=client_credentials
    - scope
    restricted: true
    restriction: approved partners only; credentials distributed by secure email
  - flow: refreshToken
    parameters:
    - grant_type=refresh_token
    - refresh_token
    - client_id
    - client_secret
    token_endpoint: https://app.401go.com/api/o/token
  header: 'Authorization: Bearer <access_token>'
  issuer: https://app.401go.com/api/o
  name: oauth2
  preferred: true
  refresh_token_lifetime_seconds: 2592000
  sources:
  - https://developer.401go.com/docs/authentication
  - https://app.401go.com/api/o/.well-known/openid-configuration
  spec_declaration:
    description: OAuth 2.0 Bearer based with an existing token. Enter a token retrieved via the regular OAuth flow elsewhere.
    note: declared as http/bearer in the spec; the real model is full OAuth 2.0
    scheme: bearer
    type: http
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- claims_supported:
  - sub
  docs: https://developer.401go.com/docs/single-sign-on-sso-with-openid-connect-oidc
  id_token_signing_algs:
  - RS256
  - HS256
  name: openIdConnect
  note: The openid scope alone grants employee (participant) access. SSO for a company admin requires openid plus company:read. company_name is populated only for company_admin; dob only for participant.
  openIdConnectUrl: https://app.401go.com/api/o/.well-known/openid-configuration
  roles:
  - participant
  - company_admin
  scope: openid
  sources:
  - https://app.401go.com/api/o/.well-known/openid-configuration
  subject_types:
  - public
  type: openIdConnect
  userinfo_claims_observed:
  - sub
  - role
  - name
  - company_name
  - dob
  - email
  - phone_number
- declared_on_operations: 50
  description: Token-based authentication with required prefix "Token" (Django REST Knox).
  documented_in_docs: false
  format: Token <token>
  in: header
  name: knoxApiToken
  note: Declared in the OpenAPI on 50 of 72 operations but never mentioned in the developer documentation. It appears to serve 401GO's own first-party clients rather than partners; partner integrations should use OAuth 2.0.
  parameter: Authorization
  sources:
  - openapi/401go-openapi-original.json
  type: apiKey
slug: 401go-authentication
source_filename: 401go-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/401go-openapi-original.json\ndocs: https://developer.401go.com/docs/authentication\nadditional_sources:\n- https://developer.401go.com/docs/client-credentials-flow\n- https://developer.401go.com/docs/single-sign-on-sso-with-openid-connect-oidc\n- https://developer.401go.com/docs/api-endpoint-and-method-access\n- https://app.401go.com/api/o/.well-known/openid-configuration\nnote: >-\n  Upgraded from derived to searched. The published OpenAPI understates the auth model: it\n  declares the OAuth surface as a bare http/bearer scheme with no flows, URLs or scopes, so a\n  spec-only derivation loses the entire authorization-code/client-credentials/OIDC picture and\n  all 12 scopes. Those are recovered here from the docs and the live authorization-server\n  metadata.\n\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  primary: oauth2\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in:\
  \ [header]\n  mtls: false\n  spec_declared_types: [apiKey, http]\n\nschemes:\n- name: oauth2\n  type: oauth2\n  preferred: true\n  spec_declaration:\n    type: http\n    scheme: bearer\n    description: >-\n      OAuth 2.0 Bearer based with an existing token. Enter a token retrieved via the regular\n      OAuth flow elsewhere.\n    note: declared as http/bearer in the spec; the real model is full OAuth 2.0\n  header: 'Authorization: Bearer <access_token>'\n  issuer: https://app.401go.com/api/o\n  endpoints:\n    authorization: https://app.401go.com/api/o/authorize\n    token: https://app.401go.com/api/o/token\n    userinfo: https://app.401go.com/api/o/userinfo\n    jwks: https://app.401go.com/api/o/.well-known/jwks.json\n    discovery: https://app.401go.com/api/o/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    preferred: true\n    parameters: [response_type=code, client_id, redirect_uri, scope, state]\n    exchange_parameters: [grant_type=authorization_code,\
  \ code, redirect_uri, client_id, client_secret]\n    pkce: true\n    code_challenge_methods: [plain, S256]\n    docs: https://developer.401go.com/docs/authentication\n    note: >-\n      If a user has multiple accounts (participant, company, advisor) they must select which\n      account to grant access to before the code is issued.\n  - flow: clientCredentials\n    restricted: true\n    restriction: approved partners only; credentials distributed by secure email\n    client_auth: 'Authorization: Basic base64(client_id:client_secret)'\n    content_type: application/x-www-form-urlencoded\n    parameters: [grant_type=client_credentials, scope]\n    docs: https://developer.401go.com/docs/client-credentials-flow\n    note: >-\n      Entities the client credentials may access are fixed during onboarding; expanding them\n      requires a request to 401GO.\n  - flow: refreshToken\n    parameters: [grant_type=refresh_token, refresh_token, client_id, client_secret]\n    token_endpoint: https://app.401go.com/api/o/token\n\
  \  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  access_token_lifetime_seconds: 3600\n  refresh_token_lifetime_seconds: 2592000\n  sources: [https://developer.401go.com/docs/authentication, https://app.401go.com/api/o/.well-known/openid-configuration]\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.401go.com/api/o/.well-known/openid-configuration\n  scope: openid\n  id_token_signing_algs: [RS256, HS256]\n  subject_types: [public]\n  claims_supported: [sub]\n  userinfo_claims_observed: [sub, role, name, company_name, dob, email, phone_number]\n  roles: [participant, company_admin]\n  note: >-\n    The openid scope alone grants employee (participant) access. SSO for a company admin\n    requires openid plus company:read. company_name is populated only for company_admin; dob\n    only for participant.\n  docs: https://developer.401go.com/docs/single-sign-on-sso-with-openid-connect-oidc\n  sources: [https://app.401go.com/api/o/.well-known/openid-configuration]\n\
  - name: knoxApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <token>'\n  description: Token-based authentication with required prefix \"Token\" (Django REST Knox).\n  declared_on_operations: 50\n  documented_in_docs: false\n  note: >-\n    Declared in the OpenAPI on 50 of 72 operations but never mentioned in the developer\n    documentation. It appears to serve 401GO's own first-party clients rather than partners;\n    partner integrations should use OAuth 2.0.\n  sources: [openapi/401go-openapi-original.json]\n\nlayered_authorization:\n  model: endpoint + HTTP-method allow list\n  enforced_in_addition_to: [oauth scopes]\n  behavior: >-\n    Each API client is explicitly granted permission for specific endpoint + HTTP-method\n    combinations. A request to a combination not on the client's allow list returns 403\n    Forbidden even with a valid, correctly scoped token. Permissions are per combination, not\n    per endpoint — GET on a path may be allowed\
  \ while POST on the same path is not.\n  granted_at: partner onboarding\n  expand_via: https://forms.gle/KQm63UQyytqTdVDe8\n  docs: https://developer.401go.com/docs/api-endpoint-and-method-access\n\nscopes:\n  count: 12\n  file: scopes/401go-scopes.yml\n  source: https://app.401go.com/api/o/.well-known/openid-configuration\n\nsecurity_application:\n  global_security_declared: false\n  note: >-\n    The spec declares no root-level security object; security is applied per operation. All 72\n    operations require oauth2; 50 also accept knoxApiToken.\n  operations_requiring_oauth2: 72\n  operations_accepting_knox: 50\n\ngaps:\n- The OpenAPI declares oauth2 as http/bearer, so no flows, endpoints or scopes are machine-readable from the spec.\n- No root-level security object in the spec.\n- Authorization-server metadata is not at the RFC 8414 well-known root path.\n- knoxApiToken is declared in the spec but undocumented.\n- No mTLS, private_key_jwt, or FAPI-grade client authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/authentication/401go-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Retirement
- 401k
- Financial Services
- Fintech
- Payroll
- Human Resources
- Benefits
- Investments
- Wealth Management
---
