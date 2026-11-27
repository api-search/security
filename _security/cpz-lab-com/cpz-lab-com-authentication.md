---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cpz-lab-com-accounts-api-openapi.yml
  format: yaml
  label: CPZ Lab Accounts API
  slug: cpz-lab-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-accounts-api-openapi.yml
- filename: cpz-lab-com-actions-api-openapi.yml
  format: yaml
  label: CPZ Lab Actions API
  slug: cpz-lab-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-actions-api-openapi.yml
- filename: cpz-lab-com-backtests-api-openapi.yml
  format: yaml
  label: CPZ Lab Backtests API
  slug: cpz-lab-com-backtests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-backtests-api-openapi.yml
- filename: cpz-lab-com-cash-api-openapi.yml
  format: yaml
  label: CPZ Lab Cash API
  slug: cpz-lab-com-cash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-cash-api-openapi.yml
- filename: cpz-lab-com-data-files-api-openapi.yml
  format: yaml
  label: CPZ Lab Data Files API
  slug: cpz-lab-com-data-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-data-files-api-openapi.yml
- filename: cpz-lab-com-me-api-openapi.yml
  format: yaml
  label: CPZ Lab Me API
  slug: cpz-lab-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-me-api-openapi.yml
- filename: cpz-lab-com-order-approvals-api-openapi.yml
  format: yaml
  label: CPZ Lab Order Approvals API
  slug: cpz-lab-com-order-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-order-approvals-api-openapi.yml
- filename: cpz-lab-com-orders-api-openapi.yml
  format: yaml
  label: CPZ Lab Orders API
  slug: cpz-lab-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-orders-api-openapi.yml
- filename: cpz-lab-com-positions-api-openapi.yml
  format: yaml
  label: CPZ Lab Positions API
  slug: cpz-lab-com-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-positions-api-openapi.yml
- filename: cpz-lab-com-risk-snapshots-api-openapi.yml
  format: yaml
  label: CPZ Lab Risk Snapshots API
  slug: cpz-lab-com-risk-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-risk-snapshots-api-openapi.yml
- filename: cpz-lab-com-strategies-api-openapi.yml
  format: yaml
  label: CPZ Lab Strategies API
  slug: cpz-lab-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-strategies-api-openapi.yml
- filename: cpz-lab-com-transactions-api-openapi.yml
  format: yaml
  label: CPZ Lab Transactions API
  slug: cpz-lab-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-transactions-api-openapi.yml
- filename: cpz-lab-com-watchlist-api-openapi.yml
  format: yaml
  label: CPZ Lab Watchlist API
  slug: cpz-lab-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-watchlist-api-openapi.yml
- filename: cpz-lab-com-webhooks-api-openapi.yml
  format: yaml
  label: CPZ Lab Webhooks API
  slug: cpz-lab-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CPZ Lab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: CPZ Lab secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: CPZ Lab
provider_slug: cpz-lab-com
scheme_count: 3
schemes:
- description: Paired with X-CPZ-Secret. Recommended for SDK and server-to-server use.
  in: header
  name: ApiKeyHeader
  parameter: X-CPZ-Key
  sources:
  - openapi/cpz-lab-com-openapi.yml
  type: apiKey
- bearerFormat: cpz_key
  description: 'Single-header API key: Authorization: Bearer cpz_key_PREFIX.SECRET'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/cpz-lab-com-openapi.yml
  type: http
- description: OAuth 2.0 + PKCE issued by the CPZAI authorization server.
  flows:
  - authorizationUrl: https://api.cpz-lab.com/oauth/authorize
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://api.cpz-lab.com/oauth/token
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://api.cpz-lab.com/oauth/token
  name: OAuth2
  sources:
  - openapi/cpz-lab-com-openapi.yml
  type: oauth2
slug: cpz-lab-com-authentication
source_filename: cpz-lab-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://ai.cpz-lab.com/docs/api/introduction\n- https://ai.cpz-lab.com/docs/sdk/authentication\n- openapi/cpz-lab-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-CPZ-Key\n  description: Paired with X-CPZ-Secret. Recommended for SDK and server-to-server use.\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: cpz_key\n  description: 'Single-header API key: Authorization: Bearer cpz_key_PREFIX.SECRET'\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cpz-lab.com/oauth/authorize\n    tokenUrl: https://api.cpz-lab.com/oauth/token\n    scopes: 12\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.cpz-lab.com/oauth/token\n    scopes: 8\n  description: OAuth 2.0 + PKCE issued by the CPZAI authorization server.\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\ndocs: https://ai.cpz-lab.com/docs/sdk/authentication\ndocumented:\n  headers:\n  - X-CPZ-Key\n  - X-CPZ-Secret\n  credential_format:\n    api_key: cpz_key_ + 24 hex characters\n    secret: cpz_secret_ + 48 alphanumeric characters\n  env_vars:\n  - CPZ_AI_API_KEY\n  - CPZ_AI_API_SECRET\n  issuance: Settings > API Keys > Create API Key; the secret is only shown once.\n  cli: Browser sign-in with token stored in the system keychain, or an API key pair.\n"
source_yaml_url: https://artifacts.apis.io/cpz-lab-com/authentication/cpz-lab-com-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Trading
- Algorithmic Trading
- Quantitative Finance
- Backtesting
- Risk Management
- Artificial Intelligence
- MCP
- Python SDK
---
