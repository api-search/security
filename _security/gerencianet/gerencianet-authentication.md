---
api_key_in: []
api_specs:
- filename: efi-cobrancas-openapi.yml
  format: yaml
  label: Efí Pay Cobranças API
  slug: efi-cobrancas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-cobrancas-openapi.yml
- filename: efi-pix-openapi.yml
  format: yaml
  label: Efí Pay Pix API
  slug: efi-pix
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pix-openapi.yml
- filename: efi-openfinance-openapi.yml
  format: yaml
  label: Efí Pay Open Finance API
  slug: efi-openfinance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-openfinance-openapi.yml
- filename: efi-contas-openapi.yml
  format: yaml
  label: Efí Pay Contas (Account Opening) API
  slug: efi-contas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-contas-openapi.yml
- filename: efi-pagamentos-openapi.yml
  format: yaml
  label: Efí Pay Pagamentos (Bill Payment) API
  slug: efi-pagamentos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pagamentos-openapi.yml
- filename: efi-extratos-openapi.yml
  format: yaml
  label: Efí Pay Extratos (Statements) API
  slug: efi-extratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-extratos-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gerencianet Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Efí Pay (Gerencianet) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Efí Pay (Gerencianet)
provider_slug: gerencianet
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://cobrancas.api.efipay.com.br/v1/authorize
  name: oauth2ClientCredentials
  sources:
  - openapi/efi-cobrancas-openapi.yml
  - openapi/efi-contas-openapi.yml
  - openapi/efi-extratos-openapi.yml
  - openapi/efi-openfinance-openapi.yml
  - openapi/efi-pagamentos-openapi.yml
  - openapi/efi-pix-openapi.yml
  type: oauth2
slug: gerencianet-authentication
source_filename: gerencianet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/efi-cobrancas-openapi.yml, openapi/efi-contas-openapi.yml, openapi/efi-extratos-openapi.yml,\n  openapi/efi-openfinance-openapi.yml, openapi/efi-pagamentos-openapi.yml, openapi/efi-pix-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cobrancas.api.efipay.com.br/v1/authorize\n    scopes: 0\n  sources:\n  - openapi/efi-cobrancas-openapi.yml\n  - openapi/efi-contas-openapi.yml\n  - openapi/efi-extratos-openapi.yml\n  - openapi/efi-openfinance-openapi.yml\n  - openapi/efi-pagamentos-openapi.yml\n  - openapi/efi-pix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/authentication/gerencianet-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- Pix
- Boleto
- Subscriptions
- Recurring Billing
- Marketplace
- Split Payments
- Open Finance
- Banking as a Service
- Account Opening
- Bill Payment
- CNAB
- Brazil
- Fintech
---
