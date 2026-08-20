---
api_key_in: []
api_specs:
- filename: romit-application-api-openapi.yml
  format: yaml
  label: Romit Application API
  slug: romit-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-application-api-openapi.yml
- filename: romit-banking-api-openapi.yml
  format: yaml
  label: Romit Banking API
  slug: romit-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-banking-api-openapi.yml
- filename: romit-identity-api-openapi.yml
  format: yaml
  label: Romit Identity API
  slug: romit-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-identity-api-openapi.yml
- filename: romit-invoice-api-openapi.yml
  format: yaml
  label: Romit Invoice API
  slug: romit-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-invoice-api-openapi.yml
- filename: romit-oauth-api-openapi.yml
  format: yaml
  label: Romit OAuth API
  slug: romit-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-oauth-api-openapi.yml
- filename: romit-plan-api-openapi.yml
  format: yaml
  label: Romit Plan API
  slug: romit-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-plan-api-openapi.yml
- filename: romit-subscription-api-openapi.yml
  format: yaml
  label: Romit Subscription API
  slug: romit-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-subscription-api-openapi.yml
- filename: romit-transfer-api-openapi.yml
  format: yaml
  label: Romit Transfer API
  slug: romit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-transfer-api-openapi.yml
- filename: romit-user-api-openapi.yml
  format: yaml
  label: Romit User API
  slug: romit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-user-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Romit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Romit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Romit
provider_slug: romit
scheme_count: 1
schemes:
- description: Romit used OAuth2. User-context flows (authorization_code / refresh_token) authorize a customer against requested scopes; the client_credentials flow issues an application access token. Access tokens are presented as an HTTP Bearer token.
  flows:
  - authorizationUrl: https://api.romit.io/v1/oauth
    flow: authorizationCode
    scopes: 15
    tokenUrl: https://api.romit.io/v1/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.romit.io/v1/oauth/token
  name: oauth2
  sources:
  - openapi/romit-openapi.yml
  type: oauth2
slug: romit-authentication
source_filename: romit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/romit-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.romit.io/v1/oauth\n    tokenUrl: https://api.romit.io/v1/oauth/token\n    scopes: 15\n  - flow: clientCredentials\n    tokenUrl: https://api.romit.io/v1/oauth/token\n    scopes: 1\n  description: Romit used OAuth2. User-context flows (authorization_code / refresh_token) authorize\n    a customer against requested scopes; the client_credentials flow issues an application access\n    token. Access tokens are presented as an HTTP Bearer token.\n  sources:\n  - openapi/romit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/authentication/romit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Fintech
- Digital Wallet
- Payment Gateway
- Merchant Services
- Chargebacks
- Fraud Prevention
- Invoicing
- Subscription
---
