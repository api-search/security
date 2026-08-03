---
api_key_in:
- header
auth_types:
- http
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Balbix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Balbix secures its APIs with http, apiKey, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Balbix
provider_slug: balbix
scheme_count: 5
schemes:
- name: BalbixBasicAuth
  scheme: basic
  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20
  surface: Balbix REST API v1
  type: http
  used_for: Exchanging static credentials for a session Authorization token at the token endpoint. Sent as HTTP Basic on GET /apis/v1/gen_token.
- format_note: The documented header value is the raw token, not an RFC 6750 "Bearer <token>" value.
  in: header
  issued_by: GET https://{tenant}.balbix.net/apis/v1/gen_token?key={CUSTOMER_KEY}
  name: BalbixAuthorizationToken
  parameter_name: Authorization
  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20
  surface: Balbix REST API v1
  ttl_note: Tokens expire after 30 minutes.
  ttl_seconds: 1800
  type: apiKey
  used_for: Session authorization on every Balbix REST API call.
- in: header
  name: BalbixClientApiKey
  parameter_name: Client-API-Key
  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20
  surface: Balbix REST API v1
  type: apiKey
  used_for: Uniquely identifies the calling customer tenant. Required in combination with the Authorization token on every endpoint.
- in: query
  name: BalbixCustomerKey
  parameter_name: key
  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20
  surface: Balbix REST API v1
  type: apiKey
  used_for: Passed to the /apis/v1/gen_token endpoint alongside HTTP Basic credentials to identify the tenant during token issuance.
- dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize
    device_authorization: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/device/authorize
    end_session: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/logout
    introspection: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/introspect
    jwks: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/keys
    registration: https://login.balbix.net/oauth2/v1/clients
    revocation: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/revoke
    token: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token
    userinfo: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/userinfo
  flows:
  - authorizationUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize
    flow: authorizationCode
    pkce: true
    pkce_methods:
    - S256
    scopes_requested_by_app:
    - openid
    - profile
    tokenUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356
  name: BalbixOkta
  openIdConnectUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/.well-known/openid-configuration
  provider: Okta
  source: well-known/balbix-openid-configuration.json
  surface: Balbix platform web application (app.balbix.net)
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
slug: balbix-authentication
source_filename: balbix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\ndocs: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\nnote: Balbix publishes no OpenAPI or Swagger document, so this profile is derived from\n  the published Balbix REST API Guide and from live, anonymous fetches of the Okta\n  OpenID Connect discovery documents at login.balbix.net. No credential values are\n  recorded here.\nsummary:\n  types:\n  - http\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  surfaces:\n  - Balbix REST API v1 (machine-to-machine, token exchange + tenant API key)\n  - Balbix platform web application (interactive, Okta OIDC single sign-on)\nschemes:\n- name: BalbixBasicAuth\n  surface: Balbix REST API v1\n  type: http\n  scheme: basic\n  used_for: Exchanging static credentials for a session Authorization token at the\n    token endpoint. Sent as HTTP Basic on\
  \ GET /apis/v1/gen_token.\n  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\n- name: BalbixAuthorizationToken\n  surface: Balbix REST API v1\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  used_for: Session authorization on every Balbix REST API call.\n  issued_by: GET https://{tenant}.balbix.net/apis/v1/gen_token?key={CUSTOMER_KEY}\n  ttl_seconds: 1800\n  ttl_note: Tokens expire after 30 minutes.\n  format_note: The documented header value is the raw token, not an RFC 6750 \"Bearer\n    <token>\" value.\n  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\n- name: BalbixClientApiKey\n  surface: Balbix REST API v1\n  type: apiKey\n  in: header\n  parameter_name: Client-API-Key\n  used_for: Uniquely identifies the calling customer tenant. Required in combination\n    with the Authorization token on every endpoint.\n  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\n- name: BalbixCustomerKey\n\
  \  surface: Balbix REST API v1\n  type: apiKey\n  in: query\n  parameter_name: key\n  used_for: Passed to the /apis/v1/gen_token endpoint alongside HTTP Basic credentials\n    to identify the tenant during token issuance.\n  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\n- name: BalbixOkta\n  surface: Balbix platform web application (app.balbix.net)\n  type: openIdConnect\n  openIdConnectUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/.well-known/openid-configuration\n  issuer: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356\n  provider: Okta\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize\n    tokenUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token\n    scopes_requested_by_app:\n    - openid\n    - profile\n    pkce: true\n    pkce_methods:\n    - S256\n  endpoints:\n    authorization: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize\n\
  \    token: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token\n    userinfo: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/userinfo\n    jwks: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/keys\n    introspection: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/introspect\n    revocation: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/revoke\n    end_session: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/logout\n    device_authorization: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/device/authorize\n    registration: https://login.balbix.net/oauth2/v1/clients\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - RS256\n  dpop_signing_alg_values_supported:\n\
  \  - RS256\n  - RS384\n  - RS512\n  - ES256\n  - ES384\n  - ES512\n  source: well-known/balbix-openid-configuration.json\ncredential_provisioning:\n  self_service: false\n  description: 'API credentials can only be created by Balbix Engineering and Balbix\n    Customer Success, and are created per customer tenant. Balbix documents that a\n    future UI update will let users create and manage their own credentials. On\n    request Balbix provides: the Base URL for the customer''s API endpoints, a static\n    username and password for the token endpoint, a Customer Key parameter for the\n    token endpoint, and a Client API Key identifying the tenant.'\n  source: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20\nsso:\n  supported: true\n  provider: Okta\n  docs: https://docs.safe.security/balbixhelp/docs/provisioning-users-for-sso-enabled-customers\naccess_control:\n  docs: https://docs.safe.security/balbixhelp/docs/access-control-list-configuration\n  project_permissions:\
  \ https://docs.safe.security/balbixhelp/docs/project-permissions-reference\nx-evidence:\n  fetched: '2026-08-02'\n  sources:\n  - url: https://docs.safe.security/balbixhelp/docs/balbix-rest-api-guide-v20.md\n    http_status: 200\n  - url: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balbix/refs/heads/main/authentication/balbix-authentication.yml
summary_line: http/apiKey/openIdConnect · 5 schemes
tags:
- Company
- Cybersecurity
- Security
- Risk Management
- Vulnerability Management
- Exposure Management
- Asset Management
- Cyber Asset Attack Surface Management
- Continuous Threat Exposure Management
- Cyber Risk Quantification
- Application Security
---
