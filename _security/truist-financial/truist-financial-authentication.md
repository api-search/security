---
api_key_in: []
api_specs:
- filename: truist-personal-small-business-accounts-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Accounts API
  slug: truist-personal-small-business-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-accounts-openapi.yml
- filename: truist-personal-small-business-transactions-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Transactions API
  slug: truist-personal-small-business-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-transactions-openapi.yml
- filename: truist-commercial-accounts-openapi.yml
  format: yaml
  label: Truist Commercial Accounts API
  slug: truist-commercial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-accounts-openapi.yml
- filename: truist-commercial-account-transactions-openapi.yml
  format: yaml
  label: Truist Commercial Account Transactions API
  slug: truist-commercial-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-account-transactions-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Truist Financial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Truist Financial secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Truist Financial
provider_slug: truist-financial
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/truist-commercial-account-transactions-openapi.yml
  - openapi/truist-commercial-accounts-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://api.truist.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/truist-personal-small-business-accounts-openapi.yml
  - openapi/truist-personal-small-business-transactions-openapi.yml
  type: oauth2
slug: truist-financial-authentication
source_filename: truist-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truist-commercial-account-transactions-openapi.yml, openapi/truist-commercial-accounts-openapi.yml,\n  openapi/truist-personal-small-business-accounts-openapi.yml, openapi/truist-personal-small-business-transactions-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.truist.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/truist-commercial-account-transactions-openapi.yml\n  - openapi/truist-commercial-accounts-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.truist.com/oauth2/authorize\n    tokenUrl: https://api.truist.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/truist-personal-small-business-accounts-openapi.yml\n  - openapi/truist-personal-small-business-transactions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/authentication/truist-financial-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Banking
- Financial Services
- Open Banking
- Commercial Banking
- Personal Banking
- Payments
- Accounts
- Transactions
- Fortune 500
---
