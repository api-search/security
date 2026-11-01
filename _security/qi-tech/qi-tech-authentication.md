---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qi-tech-openapi-generated.yml
  format: yaml
  label: QI Tech API
  slug: qi-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qi-tech/openapi/_ae-authored/qi-tech-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Qi Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: QI Tech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: QI Tech
provider_slug: qi-tech
scheme_count: 2
schemes:
- description: JSON Web Token authentication using ES512 algorithm with private key signing
  docs: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2
  evidence_url: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2
  format: Bearer {token}
  header: Authorization
  location: header
  name: JWT Authentication
  scopes: []
  type: jwt
- description: API client key used for key exchange and token generation
  docs: https://docs.qitech.com.br/documentation/primeiros_passos/troca_de_chaves
  evidence_url: https://docs.qitech.com.br/documentation/primeiros_passos/troca_de_chaves
  format:
    api_client_key: null
  header: API-CLIENT-KEY
  location: header
  name: API Client Key
  scopes: []
  type: apiKey
slug: qi-tech-authentication
source_filename: qi-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2\ndocs: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2\nschemes:\n  - type: jwt\n    name: JWT Authentication\n    description: JSON Web Token authentication using ES512 algorithm with private key signing\n    location: header\n    header: Authorization\n    format: Bearer {token}\n    scopes: []\n    docs: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2\n    evidence_url: https://docs.qitech.com.br/documentation/primeiros_passos/teste_de_autenticacao/teste_de_autenticacao_v2\n  - type: apiKey\n    name: API Client Key\n    description: API client key used for key exchange and token generation\n    location: header\n    header: API-CLIENT-KEY\n    format: {api_client_key}\n    scopes: []\n    docs: https://docs.qitech.com.br/documentation/primeiros_passos/troca_de_chaves\n\
  \    evidence_url: https://docs.qitech.com.br/documentation/primeiros_passos/troca_de_chaves\nnote: Authentication involves key exchange to obtain API-CLIENT-KEY, then JWT signing with ES512 algorithm using private key. Code examples provided in Python, PHP, Node.js, Java, C#."
source_yaml_url: https://artifacts.apis.io/qi-tech/authentication/qi-tech-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fintech
- Banking as a Service
- Lending
- Payments
- Pix
- KYC
- Fraud Prevention
- Fund Administration
- Brazil
---
