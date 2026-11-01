---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: itau-unibanco-accounts-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Accounts API
  slug: itau-unibanco-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-accounts-api-openapi.yml
- filename: itau-unibanco-channels-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Channels API
  slug: itau-unibanco-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-channels-api-openapi.yml
- filename: itau-unibanco-credit-cards-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Credit Cards API
  slug: itau-unibanco-credit-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-credit-cards-api-openapi.yml
- filename: itau-unibanco-discovery-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Discovery API
  slug: itau-unibanco-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-discovery-api-openapi.yml
- filename: itau-unibanco-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Financings API
  slug: itau-unibanco-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-financings-api-openapi.yml
- filename: itau-unibanco-invoice-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Invoice Financings API
  slug: itau-unibanco-invoice-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-invoice-financings-api-openapi.yml
- filename: itau-unibanco-loans-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Loans API
  slug: itau-unibanco-loans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-loans-api-openapi.yml
- filename: itau-unibanco-unarranged-account-overdraft-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Unarranged Account Overdraft API
  slug: itau-unibanco-unarranged-account-overdraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-unarranged-account-overdraft-api-openapi.yml
auth_types:
- apiKey
- oauth2
- mtls
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Itau Unibanco Authentication
name_suffix: Authentication
oauth_flows:
- client_credentials
overview: Itaú Unibanco secures its APIs with apiKey, oauth2, and mtls across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client_credentials flow(s).
provider_name: Itaú Unibanco
provider_slug: itau-unibanco
scheme_count: 2
schemes:
- in: query
  name: APIKey1
  parameter: API Key
  sources:
  - openapi/itau-unibanco-open-finance-opendata-accounts-openapi.yml
  - openapi/itau-unibanco-open-finance-opendata-creditcards-openapi.yml
  - openapi/itau-unibanco-open-finance-opendata-financings-openapi.yml
  - openapi/itau-unibanco-open-finance-opendata-invoicefinancings-openapi.yml
  - openapi/itau-unibanco-open-finance-opendata-loans-openapi.yml
  - openapi/itau-unibanco-open-finance-opendata-unarranged-openapi.yml
  type: apiKey
- flow: client_credentials
  mtls_required: true
  name: OAuth 2.0 Client Credentials with mTLS
  scopes: []
  sources:
  - https://devportal.itau.com.br/como-fazer-a-primeira-chamada-a-uma-api
  - https://devportal.itau.com.br/conceitos
  token_url: Not publicly documented (requires login)
  type: oauth2
slug: itau-unibanco-authentication
source_filename: itau-unibanco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://devportal.itau.com.br/como-fazer-a-primeira-chamada-a-uma-api, https://devportal.itau.com.br/conceitos, openapi/ (8 document(s))\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - mtls\n  api_key_in:\n  - query\n  oauth2_flows:\n  - client_credentials\n  mtls_required: true\nschemes:\n- name: APIKey1\n  type: apiKey\n  in: query\n  parameter: API Key\n  sources:\n  - openapi/itau-unibanco-open-finance-opendata-accounts-openapi.yml\n  - openapi/itau-unibanco-open-finance-opendata-creditcards-openapi.yml\n  - openapi/itau-unibanco-open-finance-opendata-financings-openapi.yml\n  - openapi/itau-unibanco-open-finance-opendata-invoicefinancings-openapi.yml\n  - openapi/itau-unibanco-open-finance-opendata-loans-openapi.yml\n  - openapi/itau-unibanco-open-finance-opendata-unarranged-openapi.yml\n- name: OAuth 2.0 Client Credentials with mTLS\n  type: oauth2\n  flow: client_credentials\n  token_url: Not publicly documented (requires\
  \ login)\n  scopes: []\n  mtls_required: true\n  sources:\n  - https://devportal.itau.com.br/como-fazer-a-primeira-chamada-a-uma-api\n  - https://devportal.itau.com.br/conceitos\ndocs: https://devportal.itau.com.br/como-fazer-a-primeira-chamada-a-uma-api\nnote: 'Open Finance APIs use API key authentication. Other APIs (Pix, payments, credit, etc.) use OAuth 2.0 Client Credentials with mutual TLS (mTLS) requiring dynamic certificates. Certificate generation requires login and commercial agreement.'\n"
source_yaml_url: https://artifacts.apis.io/itau-unibanco/authentication/itau-unibanco-authentication.yml
summary_line: apiKey/oauth2/mtls · 2 schemes
tags:
- Company
- Banking
- Financial Services
- Payments
- Pix
- Open Finance
- Brazil
- Foreign Exchange
- Credit
---
