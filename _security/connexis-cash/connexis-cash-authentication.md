---
anonymous_access: false
api_key_in: []
api_specs:
- filename: connexis-cash-account-information-psd2-stet-mock-openapi.yml
  format: yaml
  label: Connexis Cash PSD2 Account Information API (STET)
  slug: psd2-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml
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
mechanism_count: 1
method: derived
name: Connexis Cash Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Connexis Cash secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Connexis Cash
provider_slug: connexis-cash
scheme_count: 2
schemes:
- description: 'In order to access each of the 3 scopes in Production environment, the TPP needs to get an authorization code grant OAUTH2 token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that has been set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of https://docbox.etsi.org/ESI/'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml
  type: oauth2
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
  - openapi/connexis-cash-accounts-api-openapi.yml
  - openapi/connexis-cash-balances-api-openapi.yml
  - openapi/connexis-cash-beneficiaries-api-openapi.yml
  - openapi/connexis-cash-consents-api-openapi.yml
  - openapi/connexis-cash-transactions-api-openapi.yml
  type: oauth2
slug: connexis-cash-authentication
source_filename: connexis-cash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml, openapi/connexis-cash-accounts-api-openapi.yml,\n  openapi/connexis-cash-balances-api-openapi.yml, openapi/connexis-cash-beneficiaries-api-openapi.yml,\n  openapi/connexis-cash-consents-api-openapi.yml, openapi/connexis-cash-transactions-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token\n    scopes: 3\n  description: |-\n    In order to access each of the 3 scopes in Production environment, the TPP needs to get an authorization code grant OAUTH2 token.\n    The client_id field within the token request must be filled with the value of the organization identifier attribute that has been set in the distinguished name of eIDAS certificate of the TPP, according\
  \ to ETSI recommandations.\n    (cf §5.2.1 of https://docbox.etsi.org/ESI/\n  sources:\n  - openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n    scopes: 1\n  sources:\n  - openapi/connexis-cash-accounts-api-openapi.yml\n  - openapi/connexis-cash-balances-api-openapi.yml\n  - openapi/connexis-cash-beneficiaries-api-openapi.yml\n  - openapi/connexis-cash-consents-api-openapi.yml\n  - openapi/connexis-cash-transactions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/authentication/connexis-cash-authentication.yml
summary_line: oauth2 · 2 schemes
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
