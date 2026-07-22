---
api_key_in: []
api_specs:
- filename: mason-apps-openapi.json
  format: json
  label: Mason Apps API
  slug: mason-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-apps-openapi.json
- filename: mason-generation-openapi.json
  format: json
  label: Mason Generation API (Genie)
  slug: mason-generation-api-genie
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-generation-openapi.json
- filename: mason-tasks-openapi.json
  format: json
  label: Mason Creative Tasks API
  slug: mason-creative-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-tasks-openapi.json
- filename: mason-search-openapi.json
  format: json
  label: Mason Asset Search API
  slug: mason-asset-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-search-openapi.json
- filename: mason-webhooks-openapi.json
  format: json
  label: Mason Webhooks API
  slug: mason-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-webhooks-openapi.json
- filename: mason-discounts-openapi.json
  format: json
  label: Mason Promotion Engine API (Scrooge)
  slug: mason-promotion-engine-api-scrooge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-discounts-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mason Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Mason secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Mason
provider_slug: mason
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/mason-apps-openapi.json
  - openapi/mason-generation-openapi.json
  - openapi/mason-search-openapi.json
  - openapi/mason-webhooks-openapi.json
  type: oauth2
slug: mason-authentication
source_filename: mason-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mason-apps-openapi.json, openapi/mason-generation-openapi.json, openapi/mason-search-openapi.json,\n  openapi/mason-webhooks-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/mason-apps-openapi.json\n  - openapi/mason-generation-openapi.json\n  - openapi/mason-search-openapi.json\n  - openapi/mason-webhooks-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/authentication/mason-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ecommerce
- Commerce
- AI
- Agents
- Content Generation
- Discounts
- Promotions
- Webhooks
- Shopify
---
