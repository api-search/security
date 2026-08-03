---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Arist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- tokenExchange
- implicit
- password
overview: Arist secures its APIs with openIdConnect, oauth2, and saml across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, tokenExchange, implicit, and password flow(s).
provider_name: Arist
provider_slug: arist
scheme_count: 3
schemes:
- backchannel_logout: true
  dpop:
    signing_algs:
    - ES256
    supported: true
  dynamic_client_registration: true
  endpoints:
    authorization: https://auth.arist.app/authorize
    backchannel_authentication: https://auth.arist.app/bc-authorize
    device_authorization: https://auth.arist.app/oauth/device/code
    jwks: https://auth.arist.app/.well-known/jwks.json
    mfa_challenge: https://auth.arist.app/mfa/challenge
    registration: https://auth.arist.app/oidc/register
    revocation: https://auth.arist.app/oauth/revoke
    token: https://auth.arist.app/oauth/token
    userinfo: https://auth.arist.app/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.arist.app/
  name: AristOIDC
  openIdConnectUrl: https://auth.arist.app/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    - plain
    supported: true
  provider: Auth0
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/arist-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- description: 'Enterprise customers federate into the Arist Auth0 tenant. SAML supports both

    SP-initiated and IdP-initiated login; OIDC federation is SP-initiated only.

    '
  identity_providers:
  - Microsoft Entra ID (Azure AD)
  - Okta
  - Google Workspace
  - Active Directory / LDAP
  - ADFS
  - PingFederate
  idp_initiated: saml-only
  name: AristEnterpriseSSO
  protocols:
  - SAML 2.0
  - OpenID Connect
  sources:
  - https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide
  type: saml
- description: 'Organizations without SSO sign in with a one-time passcode delivered to their work

    email. When SSO is enabled for an organization the SSO flow always takes precedence

    and the passcode option is unavailable.

    '
  name: AristEmailPasscode
  sources:
  - https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide
  type: passwordless
slug: arist-authentication
source_filename: arist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://auth.arist.app/.well-known/openid-configuration\ndocs: https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - saml\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - deviceCode\n  - tokenExchange\n  - implicit\n  - password\n  note: |\n    Arist publishes no OpenAPI, so no securitySchemes could be derived mechanically.\n    This profile is searched: it is built from the anonymously published OIDC discovery\n    document on Arist's own Auth0 tenant plus the help-center SSO integration guide.\n    The platform API host (api.arist.app) is an Amazon API Gateway deployment that\n    answers every anonymous request with 403 MissingAuthenticationToken; the credential\n    type it expects is not publicly documented. Customer system integrations are brokered\n    by Workato, which stores\
  \ the Arist API credentials on the customer's behalf.\nschemes:\n- name: AristOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.arist.app/.well-known/openid-configuration\n  issuer: https://auth.arist.app/\n  provider: Auth0\n  endpoints:\n    authorization: https://auth.arist.app/authorize\n    token: https://auth.arist.app/oauth/token\n    userinfo: https://auth.arist.app/userinfo\n    jwks: https://auth.arist.app/.well-known/jwks.json\n    revocation: https://auth.arist.app/oauth/revoke\n    registration: https://auth.arist.app/oidc/register\n    device_authorization: https://auth.arist.app/oauth/device/code\n    backchannel_authentication: https://auth.arist.app/bc-authorize\n    mfa_challenge: https://auth.arist.app/mfa/challenge\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  pkce:\n    supported: true\n    methods: [S256, plain]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs: [HS256, RS256, PS256]\n  dpop:\n    supported: true\n    signing_algs: [ES256]\n  dynamic_client_registration: true\n  backchannel_logout: true\n  sources: [well-known/arist-openid-configuration.json]\n- name: AristEnterpriseSSO\n  type: saml\n  description: |\n    Enterprise customers federate into the Arist Auth0 tenant. SAML supports both\n    SP-initiated and IdP-initiated login; OIDC federation is SP-initiated\
  \ only.\n  protocols: [SAML 2.0, OpenID Connect]\n  identity_providers:\n  - Microsoft Entra ID (Azure AD)\n  - Okta\n  - Google Workspace\n  - Active Directory / LDAP\n  - ADFS\n  - PingFederate\n  idp_initiated: saml-only\n  sources: [https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide]\n- name: AristEmailPasscode\n  type: passwordless\n  description: |\n    Organizations without SSO sign in with a one-time passcode delivered to their work\n    email. When SSO is enabled for an organization the SSO flow always takes precedence\n    and the passcode option is unavailable.\n  sources: [https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide]\ngated_surfaces:\n- host: https://api.arist.app\n  observed: 403 MissingAuthenticationToken (Amazon API Gateway)\n  credential_type: not publicly documented\n  brokered_by: Workato\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - url: https://auth.arist.app/.well-known/openid-configuration\n\
  \    http_status: 200\n    content_type: application/json\n  - url: https://help.arist.co/article/1027-arist-application-sso-single-sign-on-integration-guide\n    http_status: 200\n  - url: https://api.arist.app/\n    http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arist/refs/heads/main/authentication/arist-authentication.yml
summary_line: openIdConnect/oauth2/saml · 3 schemes
tags:
- Company
- Learning
- Training
- Enablement
- Microlearning
- Human Resources
- Messaging
- Artificial Intelligence
- Employee Communications
- SaaS
---
