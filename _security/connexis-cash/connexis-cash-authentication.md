---
api_key_in: []
api_specs:
- filename: connexis-cash-accounts-api-openapi.yml
  format: yaml
  label: Connexis Cash Accounts API
  slug: connexis-cash-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-accounts-api-openapi.yml
- filename: connexis-cash-balances-api-openapi.yml
  format: yaml
  label: Connexis Cash Balances API
  slug: connexis-cash-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-balances-api-openapi.yml
- filename: connexis-cash-beneficiaries-api-openapi.yml
  format: yaml
  label: Connexis Cash Beneficiaries API
  slug: connexis-cash-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-beneficiaries-api-openapi.yml
- filename: connexis-cash-consents-api-openapi.yml
  format: yaml
  label: Connexis Cash Consents API
  slug: connexis-cash-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-consents-api-openapi.yml
- filename: connexis-cash-transactions-api-openapi.yml
  format: yaml
  label: Connexis Cash Transactions API
  slug: connexis-cash-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Connexis Cash Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Connexis Cash secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Connexis Cash
provider_slug: connexis-cash
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/connexis-cash-openapi.yml
  type: oauth2
slug: connexis-cash-authentication
source_filename: connexis-cash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/connexis-cash-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n    scopes: 1\n  sources:\n  - openapi/connexis-cash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/authentication/connexis-cash-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Account Information
- BNP Paribas
- Cash Management
- Corporate Banking
- Digital Banking
- Liquidity Management
- Open Banking
- Payments
- PSD2
- SCA
- STET
---
