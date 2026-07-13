---
api_key_in: []
api_specs:
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Transactions API
  slug: digits-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Source Sync API
  slug: digits-com-source-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Parties API
  slug: digits-com-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Chart of Accounts API
  slug: digits-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Financial Statements API
  slug: digits-com-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Connections API
  slug: digits-com-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Organizations API
  slug: digits-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Digits Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Digits secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Digits
provider_slug: digits-com
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code grant.
  flows:
  - authorizationUrl: https://connect.digits.com/v1/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://connect.digits.com/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/digits-com-openapi.yml
  type: oauth2
slug: digits-com-authentication
source_filename: digits-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/digits-com-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.digits.com/v1/oauth/authorize\n    tokenUrl: https://connect.digits.com/v1/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authorization code grant.\n  sources:\n  - openapi/digits-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/authentication/digits-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Bookkeeping
- Finance
- General Ledger
- AI
- FinTech
---
