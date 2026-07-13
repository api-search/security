---
api_key_in: []
api_specs:
- filename: citizens-bank-accounts-api-openapi.yml
  format: yaml
  label: Citizens Bank Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/openapi/citizens-bank-accounts-api-openapi.yml
- filename: citizens-bank-atm-locator-api-openapi.yml
  format: yaml
  label: Citizens Bank ATM Locator API
  slug: atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/openapi/citizens-bank-atm-locator-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Citizens Financial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Citizens Financial secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Citizens Financial
provider_slug: citizens-financial
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.citizensbank.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.citizensbank.com/oauth/token
  name: oauth2
  sources:
  - openapi/citizens-bank-accounts-api-openapi.yml
  type: oauth2
slug: citizens-financial-authentication
source_filename: citizens-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/citizens-bank-accounts-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.citizensbank.com/oauth/authorize\n    tokenUrl: https://api.citizensbank.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/citizens-bank-accounts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/authentication/citizens-financial-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounts
- ATMs
- Banking
- Open Banking
- Payments
- Point of Sale
- Transactions
---
