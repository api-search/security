---
api_key_in:
- header
api_specs:
- filename: 24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
  format: yaml
  label: Request Finance AP and AR API
  slug: request-finance-ap-and-ar-api
  spec_type: Postman
  url: https://www.postman.com/request-finance/workspace/request-finance-api-public/documentation/24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Request Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Request Finance secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Request Finance
provider_slug: request
scheme_count: 3
schemes:
- deprecated: true
  description: Test or live API key placed directly in the Authorization header (no "Bearer" prefix). Found in Settings > Developer > API keys. Recommended only for getting started; will be deprecated in favor of OAuth.
  in: header
  name: apiKey
  parameter_name: Authorization
  sources:
  - https://docs.request.finance/getting-started
  type: apiKey
- description: OAuth 2.0 / OpenID Connect via Auth0. Access token used as a Bearer token in the Authorization header, plus a mandatory X-Network header (test | live). Access tokens expire after 24 hours; refresh tokens (Authorization Code Flow) or client secret (Client Credentials Flow) mint new access tokens.
  flows:
  - audience: accounts
    authorizationUrl: https://auth.request.finance/authorize
    flow: authorizationCode
    tokenUrl: https://auth.request.finance/oauth/token
    use_case: Act on your users' behalf (read/manage users' invoices).
  - audience: accounts
    flow: clientCredentials
    tokenUrl: https://auth.request.finance/oauth/token
    use_case: Act on your own account's behalf (send invoices from your account).
  issuer: https://auth.request.finance
  name: oauth2
  sources:
  - https://docs.request.finance/going-live
  type: oauth2
- description: OIDC-conformant since May 2026. ID tokens signed asymmetrically (RS256). Authentication requests must include a nonce.
  name: openIdConnect
  sources:
  - https://docs.request.finance/going-live
  type: openIdConnect
slug: request-authentication
source_filename: request-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.request.finance/getting-started\ndocs: https://docs.request.finance/going-live\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  notes: >-\n    Two authentication modes. API keys (Bearer in the Authorization header) are for\n    quick starts and are being deprecated. OAuth 2.0 / OIDC via Auth0 is required for\n    production. As of May 2026 authentication is OIDC-conformant (RS256-signed ID\n    tokens, nonce required, response_type semantics changed).\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Test or live API key placed directly in the Authorization header (no \"Bearer\"\n    prefix). Found in Settings > Developer > API keys. Recommended only for getting\n    started; will be deprecated in favor of OAuth.\n  deprecated: true\n  sources: [https://docs.request.finance/getting-started]\n\
  - name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 / OpenID Connect via Auth0. Access token used as a Bearer token in the\n    Authorization header, plus a mandatory X-Network header (test | live). Access\n    tokens expire after 24 hours; refresh tokens (Authorization Code Flow) or client\n    secret (Client Credentials Flow) mint new access tokens.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.request.finance/authorize\n    tokenUrl: https://auth.request.finance/oauth/token\n    audience: accounts\n    use_case: Act on your users' behalf (read/manage users' invoices).\n  - flow: clientCredentials\n    tokenUrl: https://auth.request.finance/oauth/token\n    audience: accounts\n    use_case: Act on your own account's behalf (send invoices from your account).\n  issuer: https://auth.request.finance\n  sources: [https://docs.request.finance/going-live]\n- name: openIdConnect\n  type: openIdConnect\n  description: >-\n    OIDC-conformant since May\
  \ 2026. ID tokens signed asymmetrically (RS256).\n    Authentication requests must include a nonce.\n  sources: [https://docs.request.finance/going-live]\nheaders:\n- name: Authorization\n  required: true\n  description: API key, or \"Bearer <access_token>\" for OAuth.\n- name: X-Network\n  required: true\n  values: [test, live]\n  description: Selects the test (Sepolia) or live network for OAuth-authenticated calls.\n- name: Accept\n  required: true\n  values: [application/json]\n- name: Content-Type\n  required: true\n  values: [application/json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/request/refs/heads/main/authentication/request-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Payments
- Invoicing
- Crypto
- Web3
- Payroll
- Stablecoins
- Accounts Payable
- Accounts Receivable
- Fintech
- Blockchain
- REST API
---
