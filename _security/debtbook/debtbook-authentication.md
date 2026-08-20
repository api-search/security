---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Debtbook Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
- password
- device_code
- ciba
overview: DebtBook secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refresh_token, password, device_code, and ciba flow(s).
provider_name: DebtBook
provider_slug: debtbook
scheme_count: 1
schemes:
- endpoints:
    authorization: https://debtbook.okta.com/oauth2/v1/authorize
    end_session: https://debtbook.okta.com/oauth2/v1/logout
    jwks: https://debtbook.okta.com/oauth2/v1/keys
    token: https://debtbook.okta.com/oauth2/v1/token
    userinfo: https://debtbook.okta.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  issuer: https://debtbook.okta.com
  name: DebtBookOkta
  openIdConnectUrl: https://debtbook.okta.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  provider: Okta
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  scopes:
  - openid
  - email
  - profile
  - address
  - phone
  - offline_access
  - groups
  sources:
  - well-known/debtbook-openid-configuration.json
  - well-known/debtbook-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
slug: debtbook-authentication
source_filename: debtbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://debtbook.okta.com/.well-known/openid-configuration\ndocs: https://support.debtbook.com/en/\nnote: 'DebtBook publishes no OpenAPI, so there are no securitySchemes to derive from.\n  This profile is built from the two authorization-server metadata documents DebtBook''s\n  Okta tenant actually serves, plus the platform''s documented single sign-on support.\n  It describes how a HUMAN or an SSO-federated organization authenticates to the DebtBook\n  application — DebtBook does not publish a self-service developer credential (no API\n  key issuance, no public OAuth client registration, no documented developer token flow).'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refresh_token\n  - password\n  - device_code\n  - ciba\n  developer_credentials_published: false\n  sso: true\nschemes:\n- name: DebtBookOkta\n  type: openIdConnect\n  openIdConnectUrl:\
  \ https://debtbook.okta.com/.well-known/openid-configuration\n  issuer: https://debtbook.okta.com\n  provider: Okta\n  endpoints:\n    authorization: https://debtbook.okta.com/oauth2/v1/authorize\n    token: https://debtbook.okta.com/oauth2/v1/token\n    userinfo: https://debtbook.okta.com/oauth2/v1/userinfo\n    jwks: https://debtbook.okta.com/oauth2/v1/keys\n    end_session: https://debtbook.okta.com/oauth2/v1/logout\n  scopes:\n  - openid\n  - email\n  - profile\n  - address\n  - phone\n  - offline_access\n  - groups\n  response_types:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  pkce:\n    supported: true\n    code_challenge_methods:\n\
  \    - S256\n  sources:\n  - well-known/debtbook-openid-configuration.json\n  - well-known/debtbook-oauth-authorization-server.json\nsso:\n  supported: true\n  docs: https://support.debtbook.com/en/\n  note: DebtBook's help center carries a Single Sign-On (SSO) collection for configuring\n    organizational SSO; the article bodies are behind customer login, so the specific\n    IdP list and protocol (SAML vs OIDC) could not be confirmed anonymously.\nthird_party_data_access:\n  - name: Koxa Treasury Gateway\n    role: DebtBook's Cash Management product reaches customer bank accounts through\n      Koxa's open banking platform, not through a DebtBook-published API.\n    api_host: https://api.koxa.io\n    terms: https://www.debtbook.com/cash-management-terms-api-integration\n    evidence: window.KOXA_API_URL observed in the public application bootstrap script\n      at https://app.debtbook.com/app_vars.js\ngaps:\n- No public developer authentication documentation\n- No documented API key\
  \ or personal access token issuance\n- No public OAuth client registration or developer application console\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://debtbook.okta.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - url: https://debtbook.okta.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debtbook/refs/heads/main/authentication/debtbook-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Treasury Management
- Government
- Public Finance
- Debt Management
- Cash Management
- Accounting
- Lease Accounting
- Investment Management
- Non-Profit
- Higher Education
- Healthcare
- Software-as-a-Service
---
