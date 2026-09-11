---
anonymous_access: false
api_key_in:
- cookie
auth_types:
- oauth2
- apiKey
- saml2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Advicepay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: AdvicePay secures its APIs with oauth2, apiKey, and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: AdvicePay
provider_slug: advicepay
scheme_count: 3
schemes:
- bearer_header: 'Authorization: Bearer <access_token>'
  description: OAuth 2.0 is the mechanism for all public API access. Access tokens are presented in the Authorization header as "Bearer <token>".
  flows:
  - authorizationUrl: https://app.advicepay.com/oauth2/authorize
    authorization_code_ttl_seconds: 600
    description: For user-level integrations where AdvicePay users sit in different accounts. OAuth clients for firms with developer access are created in the developer console; partner clients are provisioned on request (company name, website URL, logo and redirect URI required).
    flow: authorizationCode
    refreshUrl: https://app.advicepay.com/oauth2/access_token
    state_parameter: supported (optional, CSRF protection)
    tokenUrl: https://app.advicepay.com/oauth2/access_token
  - description: For enterprise account-owner accounts acting on behalf of an integrating system. Enabled per OAuth client with the "Enable OAuth 2.0 Client Credentials Flow" toggle.
    flow: clientCredentials
    tokenUrl: https://app.advicepay.com/oauth2/access_token
  name: OAuth2
  type: oauth2
- description: Session-based authentication using a secure HTTP-only cookie (browser sessions).
  in: cookie
  name: SessionCookie
  parameter_name: session
  type: apiKey
- description: SAML 2.0 single sign-on. POST /auth/sso consumes a SAMLResponse plus RelayState and creates a session, keyed by a `source` company slug that selects the certificate to validate against. The integrator's public certificate must be installed on an AdvicePay server first (enterprise@advicepay.com). GET /auth/sso supports deep linking into the application.
  endpoints:
  - POST /auth/sso
  - GET /auth/sso
  name: SAML2 SSO
  type: saml2
slug: advicepay-authentication
source_filename: advicepay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://docs.advicepay.com/#authentication\ndocs: https://docs.advicepay.com/#authentication\nnote: >-\n  Derived by reading the published AdvicePay API documentation, not from a machine-readable\n  OpenAPI document — AdvicePay publishes no OpenAPI/Swagger file (see x-contract-discovery in\n  apis.yml). Every scheme, endpoint, lifetime and claim below is stated verbatim in the docs.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - saml2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  client_authentication_methods:\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 is the mechanism for all public API access. Access tokens are presented in the\n    Authorization header as \"Bearer <token>\".\n  bearer_header: 'Authorization: Bearer <access_token>'\n  flows:\n  - flow: authorizationCode\n  \
  \  description: >-\n      For user-level integrations where AdvicePay users sit in different accounts. OAuth clients\n      for firms with developer access are created in the developer console; partner clients are\n      provisioned on request (company name, website URL, logo and redirect URI required).\n    authorizationUrl: https://app.advicepay.com/oauth2/authorize\n    tokenUrl: https://app.advicepay.com/oauth2/access_token\n    refreshUrl: https://app.advicepay.com/oauth2/access_token\n    authorization_code_ttl_seconds: 600\n    state_parameter: supported (optional, CSRF protection)\n  - flow: clientCredentials\n    description: >-\n      For enterprise account-owner accounts acting on behalf of an integrating system. Enabled\n      per OAuth client with the \"Enable OAuth 2.0 Client Credentials Flow\" toggle.\n    tokenUrl: https://app.advicepay.com/oauth2/access_token\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter_name: session\n  description: Session-based authentication\
  \ using a secure HTTP-only cookie (browser sessions).\n- name: SAML2 SSO\n  type: saml2\n  description: >-\n    SAML 2.0 single sign-on. POST /auth/sso consumes a SAMLResponse plus RelayState and creates a\n    session, keyed by a `source` company slug that selects the certificate to validate against.\n    The integrator's public certificate must be installed on an AdvicePay server first\n    (enterprise@advicepay.com). GET /auth/sso supports deep linking into the application.\n  endpoints:\n  - POST /auth/sso\n  - GET /auth/sso\ntoken_lifetimes:\n  access_token_seconds: 300\n  access_token_note: Access tokens expire after 5 minutes (both flows).\n  refresh_token_days: 30\n  refresh_token_rotation: >-\n    Refresh tokens are single-use. A new refresh token is issued every time one is consumed and\n    the previous one is invalidated, so the integrator must persist the new token after every\n    refresh call.\n  authorization_code_seconds: 600\nclient_authentication_methods:\n- id: client_secret_post\n\
  \  description: >-\n    Client secret sent in the request body as `client_secret`. The docs describe this as the\n    least secure of the three methods.\n  security_posture: lowest\n- id: client_secret_jwt\n  description: >-\n    A JWT signed with the client secret using HS256, sent as `client_assertion` with\n    client_assertion_type urn:ietf:params:oauth:client-assertion-type:jwt-bearer. The secret\n    never leaves the integrator's server.\n  algorithm: HS256\n  security_posture: better\n- id: private_key_jwt\n  description: >-\n    A JWT signed with the integrator's private key using RS256; the public key is uploaded in the\n    developer dashboard and AdvicePay verifies each request against it. The docs describe this as\n    the most secure method.\n  algorithm: RS256\n  security_posture: highest\njwt_client_assertion:\n  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n  standard: RFC 7523 (JWT profile for OAuth 2.0 client authentication)\n  claims:\n\
  \  - claim: aud\n    required: true\n    description: The URL of the resource being authenticated to, generally https://app.advicepay.com/oauth2/access_token\n  - claim: exp\n    required: true\n    description: Expiration time; requests received after exp are rejected. Short lifetimes recommended.\n  - claim: iat\n    required: true\n    description: Issued-at time; requests received before iat are rejected.\n  - claim: iss\n    required: true\n    description: Issuer — always the client ID.\n  - claim: sub\n    required: true\n    description: Subject — always the client ID.\n  - claim: jti\n    required: false\n    description: >-\n      Token identifier. When present AdvicePay prevents the same jti being replayed, mitigating\n      replay attacks. The docs highly recommend it.\nscopes:\n  supported:\n  - all\n  note: The docs state that only the scope value \"all\" is currently supported.\ndeveloper_console: >-\n  OAuth clients, the client-credentials toggle, the client authentication\
  \ method and the\n  private-key JWT public key are all managed in the AdvicePay developer console, available to\n  firms with developer access (an Enterprise-plan capability). Partner/integration clients are\n  provisioned on request via enterprise@advicepay.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advicepay/refs/heads/main/authentication/advicepay-authentication.yml
summary_line: oauth2/apiKey/saml2 · 3 schemes
tags:
- Financial Services
- Payments
- Billing
- Invoicing
- Financial Planning
- Wealth Management
- Subscriptions
- eSignature
- Compliance
- FinTech
---
