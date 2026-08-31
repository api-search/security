---
api_key_in: []
api_specs:
- filename: crm-bonus-auth-api-openapi.yml
  format: yaml
  label: CRM Bonus Auth API
  slug: crm-bonus-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-auth-api-openapi.yml
- filename: crm-bonus-blocked-api-openapi.yml
  format: yaml
  label: CRM Bonus Blocked API
  slug: crm-bonus-blocked-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-blocked-api-openapi.yml
- filename: crm-bonus-cashback-api-openapi.yml
  format: yaml
  label: CRM Bonus Cashback API
  slug: crm-bonus-cashback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-cashback-api-openapi.yml
- filename: crm-bonus-customers-api-openapi.yml
  format: yaml
  label: CRM Bonus Customers API
  slug: crm-bonus-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-customers-api-openapi.yml
- filename: crm-bonus-nps-api-openapi.yml
  format: yaml
  label: CRM Bonus Nps API
  slug: crm-bonus-nps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-nps-api-openapi.yml
- filename: crm-bonus-order-items-api-openapi.yml
  format: yaml
  label: CRM Bonus Order Items API
  slug: crm-bonus-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-order-items-api-openapi.yml
- filename: crm-bonus-orders-api-openapi.yml
  format: yaml
  label: CRM Bonus Orders API
  slug: crm-bonus-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-orders-api-openapi.yml
- filename: crm-bonus-products-api-openapi.yml
  format: yaml
  label: CRM Bonus Products API
  slug: crm-bonus-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-products-api-openapi.yml
- filename: crm-bonus-sellers-api-openapi.yml
  format: yaml
  label: CRM Bonus Sellers API
  slug: crm-bonus-sellers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-sellers-api-openapi.yml
- filename: crm-bonus-stores-api-openapi.yml
  format: yaml
  label: CRM Bonus Stores API
  slug: crm-bonus-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-stores-api-openapi.yml
- filename: crm-bonus-tag-hits-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Hits API
  slug: crm-bonus-tag-hits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-hits-api-openapi.yml
- filename: crm-bonus-tag-ids-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Ids API
  slug: crm-bonus-tag-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-ids-api-openapi.yml
- filename: crm-bonus-tag-interactions-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Interactions API
  slug: crm-bonus-tag-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-interactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Crm Bonus Authentication
name_suffix: Authentication
oauth_flows: []
overview: CRM Bonus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CRM Bonus
provider_slug: crm-bonus
scheme_count: 1
schemes:
- applied_to: 'All 12 /v1/* ingestion operations declare security: [{HTTPBearer: []}]. POST /auth/login is the one unauthenticated operation.'
  bearer_format: JWT
  description: 'Você deverá enviar sua chave privada

    no cabeçalho HTTP `Authorization`, com o padrão `Bearer <token>`. Exemplo:


    ```

    GET / HTTP/1.1

    Host: data-api.otocrm.com.br

    Authorization: Bearer abcdef123456

    ```'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/crm-bonus-oto-data-api-openapi.yml
  type: http
slug: crm-bonus-authentication
source_filename: crm-bonus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/crm-bonus-oto-data-api-openapi.yml\ndocs: https://ajuda.otocrm.com.br/support/solutions/articles/150000031734-cadastro-r%C3%A1pido-via-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  scopes: 0\n  note: >-\n    Single-scheme, single-credential model. No OAuth 2.0, no OpenID Connect, no\n    API-key header, no mTLS, and therefore no scope surface — which is why this\n    repo emits no scopes/ artifact.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: |-\n    Você deverá enviar sua chave privada\n    no cabeçalho HTTP `Authorization`, com o padrão `Bearer <token>`. Exemplo:\n\n    ```\n    GET / HTTP/1.1\n    Host: data-api.otocrm.com.br\n    Authorization: Bearer abcdef123456\n    ```\n  applied_to: >-\n    All 12 /v1/* ingestion operations declare security: [{HTTPBearer: []}].\n    POST /auth/login is the one unauthenticated\
  \ operation.\n  sources:\n  - openapi/crm-bonus-oto-data-api-openapi.yml\ntoken_issuance:\n  self_service: false\n  process: >-\n    \"Solicite ao time de suporte o token de acesso para utilização da API\n    pública\" — the access token is requested from Oto/CRMBonus support. There is\n    no developer portal, no key-management console and no self-serve sign-up.\n  per_environment: true\n  per_environment_note: >-\n    Production and homologação require separate credentials\n    (\"Ambos os ambientes requerem credenciais específicas\").\n  login_endpoint:\n    operation_id: login_auth_login_post\n    path: POST /auth/login\n    request: 'LoginRequest {username, password}'\n    response: 'TokenResponse {access_token, expires_in}'\n    token_type: JWT\n    expires_in: 3600\n    claims_note: >-\n      The operation description states the JWT carries user information and\n      permissions, and that credentials are validated against a `users`\n      collection. Those permissions are not exposed\
  \ as OAuth scopes and are not\n      documented anywhere public.\n    failure_modes:\n    - status: 401\n      meaning: Credenciais inválidas\n    - status: 403\n      meaning: Conta de usuário inativa\n    - status: 500\n      meaning: Erro interno por exceção não esperada\nruntime_behaviour:\n  missing_credential:\n    status: 403\n    body: '{\"detail\": \"Not authenticated\"}'\n    observed: '2026-08-12'\n    note: >-\n      403 rather than 401, and no WWW-Authenticate challenge header is returned.\n      A client that branches on 401 for \"needs auth\" will mis-handle this API.\n  transport:\n    https_only: true\n    hsts: 'max-age=31536000; includeSubDomains'\nother_surfaces:\n- name: CRMBonus Giftback / Vale Bonus API\n  host: api.crmbonus.com\n  documented: false\n  auth: >-\n    Partner-issued token. Third-party integration docs state the brand must ask\n    the CRM&Bônus team to create a token, scoped to stores and with CPF\n    collection enabled. No public reference, no published\
  \ header name, no spec.\n  note: >-\n    Recorded for completeness; not part of the derived scheme set because no\n    machine-readable contract exists for it.\ngaps:\n- No OAuth 2.0 or OIDC — no /.well-known/openid-configuration on any host (404).\n- No documented token rotation, revocation or expiry policy for support-issued tokens.\n- No WWW-Authenticate header on an unauthenticated request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/authentication/crm-bonus-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Retail
- Loyalty
- Cashback
- CRM
- Retail Media
- E-Commerce
- Brazil
- WhatsApp
- Customer Data
- Data Ingestion
- Point-of-Sale
---
