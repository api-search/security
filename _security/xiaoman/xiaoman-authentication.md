---
api_key_in:
- header
api_specs:
- filename: xiaoman-openapi.yml
  format: yaml
  label: Xiaoman OKKI CRM Open API
  slug: xiaoman-okki-crm-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-openapi.yml
- filename: xiaoman-okki-go-openapi.yml
  format: yaml
  label: OKKI Go API
  slug: okki-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-okki-go-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Xiaoman Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: Xiaoman (OKKI) secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: Xiaoman (OKKI)
provider_slug: xiaoman
scheme_count: 2
schemes:
- api: Xiaoman OKKI CRM Open API
  description: OAuth2 token issued by POST /v1/oauth2/access_token on https://api-sandbox.xiaoman.cn. Supports grant_type password (username = Xiaoman login email, password SHA-256 hashed) and client_credentials. client_id and client_secret come from the OKKI CRM admin console (企业管理 → 外部对接 → API对接). Tokens are Bearer, valid 8 hours (expires_in 28800); password grant also returns a refresh_token (refresh endpoint documented separately). client_credentials responses carry no expires_in/refresh_token — re-request before expiry. The scope parameter is a space-separated list of module scopes (see scopes/xiaoman-scopes.yml); calls outside granted scopes fail with "no permission <module> scopes".
  flows:
  - flow: password
    tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token
  header: Authorization
  name: XiaomanOAuth2
  token_lifetime_seconds: 28800
  type: oauth2
- api: OKKI Go API
  description: 'API key auth for https://go.okki.ai — header form "Authorization: ApiKey sk-...". Keys are issued at https://go.okki.ai after registration; the OKKI Go Agent Skill caches the key in ~/.config/okki-go/credentials.json (mode 0600) via its okki-auth.js helper. All authenticated endpoints share a 60 requests/minute rate limit.'
  in: header
  name: OkkiGoApiKey
  parameter: Authorization
  type: apiKey
slug: xiaoman-authentication
source_filename: xiaoman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://open.xiaoman.cn/api-3473041 and npm @okki-global/okki-go skill/references/api-reference.md\ndocs:\n  - https://open.xiaoman.cn/api-3473041\n  - https://open.xiaoman.cn/doc-338276\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [password, clientCredentials]\n  api_key_in: [header]\nschemes:\n  - name: XiaomanOAuth2\n    api: Xiaoman OKKI CRM Open API\n    type: oauth2\n    description: >-\n      OAuth2 token issued by POST /v1/oauth2/access_token on\n      https://api-sandbox.xiaoman.cn. Supports grant_type password (username =\n      Xiaoman login email, password SHA-256 hashed) and client_credentials.\n      client_id and client_secret come from the OKKI CRM admin console\n      (企业管理 → 外部对接 → API对接). Tokens are Bearer, valid 8 hours\n      (expires_in 28800); password grant also returns a refresh_token\n      (refresh endpoint documented separately). client_credentials responses\n      carry no expires_in/refresh_token\
  \ — re-request before expiry. The scope\n      parameter is a space-separated list of module scopes (see\n      scopes/xiaoman-scopes.yml); calls outside granted scopes fail with\n      \"no permission <module> scopes\".\n    flows:\n      - flow: password\n        tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token\n      - flow: clientCredentials\n        tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token\n    token_lifetime_seconds: 28800\n    header: Authorization\n  - name: OkkiGoApiKey\n    api: OKKI Go API\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      API key auth for https://go.okki.ai — header form\n      \"Authorization: ApiKey sk-...\". Keys are issued at https://go.okki.ai\n      after registration; the OKKI Go Agent Skill caches the key in\n      ~/.config/okki-go/credentials.json (mode 0600) via its okki-auth.js\n      helper. All authenticated endpoints share a 60 requests/minute rate\n      limit.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/authentication/xiaoman-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- CRM
- Foreign Trade
- B2B
- Sales
- Prospecting
- Email Marketing
- AI Agents
- China
- Alibaba
---
