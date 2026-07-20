---
api_key_in: []
api_specs:
- filename: conta-azul-acquittance-openapi.yml
  format: yaml
  label: Conta Azul Baixas (Acquittance)
  slug: conta-azul-baixas-acquittance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-acquittance-openapi.yml
- filename: conta-azul-charge-openapi.yml
  format: yaml
  label: Conta Azul Cobranças (Charges)
  slug: conta-azul-cobranças-charges
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-charge-openapi.yml
- filename: conta-azul-contracts-openapi.yml
  format: yaml
  label: Conta Azul Contratos (Contracts)
  slug: conta-azul-contratos-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-contracts-openapi.yml
- filename: conta-azul-financial-openapi.yml
  format: yaml
  label: Conta Azul Financeiro (Financial)
  slug: conta-azul-financeiro-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-financial-openapi.yml
- filename: conta-azul-inventory-openapi.yml
  format: yaml
  label: Conta Azul Produtos (Inventory)
  slug: conta-azul-produtos-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-inventory-openapi.yml
- filename: conta-azul-proposal-openapi.yml
  format: yaml
  label: Conta Azul Orçamentos (Proposals)
  slug: conta-azul-orçamentos-proposals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-proposal-openapi.yml
- filename: conta-azul-protocol-openapi.yml
  format: yaml
  label: Conta Azul Protocolos (Protocol)
  slug: conta-azul-protocolos-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-protocol-openapi.yml
- filename: conta-azul-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas (Sales)
  slug: conta-azul-vendas-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-sales-openapi.yml
- filename: conta-azul-scheduled-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas Programadas (Scheduled Sales)
  slug: conta-azul-vendas-programadas-scheduled-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-scheduled-sales-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Conta Azul Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Conta Azul secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Conta Azul
provider_slug: conta-azul
scheme_count: 2
schemes:
- access_token_ttl_seconds: 3600
  client_auth: Basic (base64 client_id:client_secret) at the token endpoint
  discovery:
    authorization_endpoint: https://api-v2.contaazul.com/oauth/authorize
    grant_types_supported:
    - authorization_code
    - refresh_token
    id_token_signing_alg: RS256
    issuer: https://api-v2.contaazul.com
    jwks_uri: https://api-v2.contaazul.com/.well-known/jwks.json
    note: RFC 8414 / OIDC discovery documents are live and advertise the endpoints on api-v2.contaazul.com; the human docs walk the same flow via auth.contaazul.com (the Cognito-fronted login/token host).
    pkce: S256
    registration_endpoint: https://api-v2.contaazul.com/oauth2/register
    source: well-known/conta-azul-openid-configuration.json + well-known/conta-azul-oauth-authorization-server.json
    token_endpoint: https://api-v2.contaazul.com/oauth/token
    userinfo_endpoint: https://api-v2.contaazul.com/v1/pessoas/conta-conectada
  flows:
  - authorizationUrl: https://auth.contaazul.com/login
    flow: authorizationCode
    scopes:
      aws.cognito.signin.user.admin: Full administrative access to all API contexts
      openid: OpenID Connect authentication
      profile: Access to the connected user profile
    tokenUrl: https://auth.contaazul.com/oauth2/token
  name: OAuth2
  refresh_token_ttl: up to 5 years / rotated on each refresh
  source: docs (https://developers.contaazul.com/auth)
  type: oauth2
- bearerFormat: JWT
  description: Bearer JWT access token sent in the Authorization header on every API call.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/conta-azul-acquittance-openapi.yml
  - openapi/conta-azul-charge-openapi.yml
  - openapi/conta-azul-contracts-openapi.yml
  - openapi/conta-azul-financial-openapi.yml
  - openapi/conta-azul-inventory-openapi.yml
  - openapi/conta-azul-protocol-openapi.yml
  - openapi/conta-azul-sales-openapi.yml
  - openapi/conta-azul-proposal-openapi.yml
  - openapi/conta-azul-scheduled-sales-openapi.yml
  type: http
slug: conta-azul-authentication
source_filename: conta-azul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/*.yml securitySchemes + https://developers.contaazul.com/auth\ndocs: https://developers.contaazul.com/auth\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  token_format: JWT\n  token_type: Bearer\nnotes: >-\n  The Conta Azul \"Nova API\" (v2, api-v2.contaazul.com) is protected by OAuth 2.0\n  Authorization Code flow on AWS Cognito (auth.contaazul.com). The OpenAPI specs\n  only declare the resulting bearer scheme (HTTP bearer, JWT), but the access\n  token is obtained through the documented OAuth2 flow. The legacy API\n  (devdocs.contaazul.com) used incompatible credentials and was sunset\n  2025-11-05.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: docs (https://developers.contaazul.com/auth)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.contaazul.com/login\n    tokenUrl: https://auth.contaazul.com/oauth2/token\n    scopes:\n \
  \     openid: OpenID Connect authentication\n      profile: Access to the connected user profile\n      aws.cognito.signin.user.admin: Full administrative access to all API contexts\n  client_auth: Basic (base64 client_id:client_secret) at the token endpoint\n  access_token_ttl_seconds: 3600\n  refresh_token_ttl: up to 5 years / rotated on each refresh\n  discovery:\n    source: well-known/conta-azul-openid-configuration.json + well-known/conta-azul-oauth-authorization-server.json\n    issuer: https://api-v2.contaazul.com\n    authorization_endpoint: https://api-v2.contaazul.com/oauth/authorize\n    token_endpoint: https://api-v2.contaazul.com/oauth/token\n    jwks_uri: https://api-v2.contaazul.com/.well-known/jwks.json\n    userinfo_endpoint: https://api-v2.contaazul.com/v1/pessoas/conta-conectada\n    registration_endpoint: https://api-v2.contaazul.com/oauth2/register\n    pkce: S256\n    id_token_signing_alg: RS256\n    grant_types_supported: [authorization_code, refresh_token]\n  \
  \  note: >-\n      RFC 8414 / OIDC discovery documents are live and advertise the endpoints on\n      api-v2.contaazul.com; the human docs walk the same flow via\n      auth.contaazul.com (the Cognito-fronted login/token host).\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer JWT access token sent in the Authorization header on every API call.\n  sources:\n  - openapi/conta-azul-acquittance-openapi.yml\n  - openapi/conta-azul-charge-openapi.yml\n  - openapi/conta-azul-contracts-openapi.yml\n  - openapi/conta-azul-financial-openapi.yml\n  - openapi/conta-azul-inventory-openapi.yml\n  - openapi/conta-azul-protocol-openapi.yml\n  - openapi/conta-azul-sales-openapi.yml\n  - openapi/conta-azul-proposal-openapi.yml\n  - openapi/conta-azul-scheduled-sales-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/authentication/conta-azul-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Fintech
- Accounting
- ERP
- Brazil
- Small Business
- Financial Management
- Invoicing
- Payments
---
