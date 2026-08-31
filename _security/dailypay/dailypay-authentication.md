---
api_key_in: []
api_specs:
- filename: dailypay-accounts-api-openapi.yml
  format: yaml
  label: DailyPay Accounts API
  slug: dailypay-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-accounts-api-openapi.yml
- filename: dailypay-card-tokenization-api-openapi.yml
  format: yaml
  label: DailyPay Card Tokenization API
  slug: dailypay-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-card-tokenization-api-openapi.yml
- filename: dailypay-health-api-openapi.yml
  format: yaml
  label: DailyPay Health API
  slug: dailypay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-health-api-openapi.yml
- filename: dailypay-jobs-api-openapi.yml
  format: yaml
  label: DailyPay Jobs API
  slug: dailypay-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-jobs-api-openapi.yml
- filename: dailypay-organizations-api-openapi.yml
  format: yaml
  label: DailyPay Organizations API
  slug: dailypay-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-organizations-api-openapi.yml
- filename: dailypay-paychecks-api-openapi.yml
  format: yaml
  label: DailyPay Paychecks API
  slug: dailypay-paychecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-paychecks-api-openapi.yml
- filename: dailypay-people-api-openapi.yml
  format: yaml
  label: DailyPay People API
  slug: dailypay-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-people-api-openapi.yml
- filename: dailypay-transfers-api-openapi.yml
  format: yaml
  label: DailyPay Transfers API
  slug: dailypay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-transfers-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Dailypay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: DailyPay secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: DailyPay
provider_slug: dailypay
scheme_count: 2
schemes:
- audience: partner application (server-to-server)
  docs: https://developer.dailypay.com/products/rest/guides/auth/client-credentials-flow
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.dailypay.com/oauth2/token
  name: oauth_client_credentials_token
  sources:
  - openapi/dailypay-rest-openapi-original.yml
  type: oauth2
- audience: employee (resource owner) via the partner application
  docs: https://developer.dailypay.com/products/rest/guides/auth/authorization-code-flow
  flows:
  - authorizationUrl: https://auth.dailypay.com/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://auth.dailypay.com/oauth2/token
  name: oauth_user_token
  pkce: true
  sources:
  - openapi/dailypay-rest-openapi-original.yml
  type: oauth2
slug: dailypay-authentication
source_filename: dailypay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/dailypay-rest-openapi-original.yml\ndocs: https://developer.dailypay.com/products/rest/guides/auth\ndiscovery: https://auth.dailypay.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  api_key_in: []\n  bearer: 'Authorization: Bearer <access_token>'\n  authorization_server: https://auth.dailypay.com\n  self_serve: false\nstatement: >-\n  \"DailyPay adheres to the OAuth 2.0 RFC 6749 and OpenID Connect specifications.\" Two token\n  acquisition paths are supported: authorization code (when the operation acts on behalf of an\n  employee and requires their consent) and client credentials (for server-to-server operations such\n  as reading connected employer organizations).\nschemes:\n- name: oauth_client_credentials_token\n  type: oauth2\n  audience: partner application (server-to-server)\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.dailypay.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n  docs: https://developer.dailypay.com/products/rest/guides/auth/client-credentials-flow\n- name: oauth_user_token\n  type: oauth2\n  audience: employee (resource owner) via the partner application\n  pkce: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.dailypay.com/oauth2/auth\n    tokenUrl: https://auth.dailypay.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n  docs: https://developer.dailypay.com/products/rest/guides/auth/authorization-code-flow\nopenid_connect:\n  supported: true\n  issuer: https://auth.dailypay.com\n  discovery: https://auth.dailypay.com/.well-known/openid-configuration\n  jwks_uri: https://auth.dailypay.com/.well-known/jwks.json\n  userinfo_endpoint: https://auth.dailypay.com/userinfo\n  revocation_endpoint: https://auth.dailypay.com/oauth2/revoke\n  end_session_endpoint:\
  \ https://auth.dailypay.com/oauth2/sessions/logout\n  id_token_signing: [RS256]\n  code_challenge_methods:\n  - S256\n  - plain\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  grant_types:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  signed_request_objects: true\n  request_uri_registration_required: true\n  logout:\n    backchannel: true\n    frontchannel: true\nfederation:\n  saml2: true\n  oidc_trust_relationship: true\n  docs: https://developer.dailypay.com/products/rest/guides/auth/trust-relationship\n  note: >-\n    DailyPay supports a \"trust relationship\" configuration in which the partner's own IdP asserts\n    the user, reducing the consent burden when embedding Elements. Partners may supply a JWKS or\n    JWKS URL so DailyPay can verify signed OIDC requests.\nrefresh:\n  supported: true\n  scope_required: offline_access\n  docs: https://developer.dailypay.com/products/rest/guides/auth/refresh-token\n\
  onboarding:\n  self_serve: false\n  process: >-\n    A DailyPay contact registers the application. The partner supplies a callback URL for the\n    authorization-code flow, links to its privacy policy and terms of service, and optionally a\n    logo for the consent screen and a JWKS for signed OIDC requests. DailyPay returns client_id,\n    client_secret (when applicable), the permitted scope list, and the registered redirect_uri.\n  registration_page: https://www.dailypay.com/developer/\nerrors:\n  '401':\n  - INVALID_TOKEN\n  - UNAUTHORIZED\n  '403':\n  - FORBIDDEN\n  artifact: errors/dailypay-problem-types.yml\nrelated:\n  scopes: scopes/dailypay-scopes.yml\n  conventions: conventions/dailypay-conventions.yml\n  well_known: well-known/dailypay-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/authentication/dailypay-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Payments
- Payroll
- Human Resources
- Earned Wage Access
- On-Demand Pay
- Financial-Services
- Fintech
- Money Transfer
- Benefits
---
