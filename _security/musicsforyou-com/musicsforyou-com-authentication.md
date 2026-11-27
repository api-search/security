---
anonymous_access: false
api_key_in: []
api_specs:
- filename: musicsforyou-com-account-api-openapi.yml
  format: yaml
  label: 桃源 Account API
  slug: musicsforyou-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-account-api-openapi.yml
- filename: musicsforyou-com-billing-api-openapi.yml
  format: yaml
  label: 桃源 Billing API
  slug: musicsforyou-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-billing-api-openapi.yml
- filename: musicsforyou-com-catalog-api-openapi.yml
  format: yaml
  label: 桃源 Catalog API
  slug: musicsforyou-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-catalog-api-openapi.yml
- filename: musicsforyou-com-compose-api-openapi.yml
  format: yaml
  label: 桃源 Compose API
  slug: musicsforyou-com-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-compose-api-openapi.yml
- filename: musicsforyou-com-edit-api-openapi.yml
  format: yaml
  label: 桃源 Edit API
  slug: musicsforyou-com-edit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-edit-api-openapi.yml
- filename: musicsforyou-com-generate-api-openapi.yml
  format: yaml
  label: 桃源 Generate API
  slug: musicsforyou-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-generate-api-openapi.yml
- filename: musicsforyou-com-keys-api-openapi.yml
  format: yaml
  label: 桃源 Keys API
  slug: musicsforyou-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-keys-api-openapi.yml
- filename: musicsforyou-com-library-api-openapi.yml
  format: yaml
  label: 桃源 Library API
  slug: musicsforyou-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-library-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: 桃源 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 桃源 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 桃源
provider_slug: musicsforyou-com
scheme_count: 2
schemes:
- bearerFormat: ty_live_…
  description: '开发者 API Key，以 `ty_live_` 开头，在 https://www.musicsforyou.com/developers 创建。请求头 `Authorization: Bearer ty_live_…`。


    API keys start with `ty_live_`; create one at https://www.musicsforyou.com/developers. Send as `Authorization: Bearer ty_live_…`.'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/musicsforyou-com-openapi.json
  type: http
- description: 给 ChatGPT / claude.ai 等连接器用的授权码流程 / Authorization-code flow for connector platforms.
  flows:
  - authorizationUrl: https://www.musicsforyou.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.musicsforyou.com/oauth/token
  name: OAuth2
  sources:
  - openapi/musicsforyou-com-openapi.json
  type: oauth2
slug: musicsforyou-com-authentication
source_filename: musicsforyou-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/musicsforyou-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: ty_live_…\n  description: |-\n    开发者 API Key，以 `ty_live_` 开头，在 https://www.musicsforyou.com/developers 创建。请求头 `Authorization: Bearer ty_live_…`。\n\n    API keys start with `ty_live_`; create one at https://www.musicsforyou.com/developers. Send as `Authorization: Bearer ty_live_…`.\n  sources:\n  - openapi/musicsforyou-com-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.musicsforyou.com/oauth/authorize\n    tokenUrl: https://api.musicsforyou.com/oauth/token\n    scopes: 1\n  description: 给 ChatGPT / claude.ai 等连接器用的授权码流程 / Authorization-code flow for connector platforms.\n  sources:\n  - openapi/musicsforyou-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/musicsforyou-com/authentication/musicsforyou-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
---
