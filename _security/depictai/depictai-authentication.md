---
api_key_in:
- cookie
- header
- query
api_specs:
- filename: depictai-storefront-openapi.json
  format: json
  label: Depict Storefront API
  slug: depict-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-storefront-openapi.json
- filename: depictai-portal-openapi.json
  format: json
  label: Depict Portal API
  slug: depict-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-portal-openapi.json
- filename: depictai-lite-openapi.json
  format: json
  label: Depict Lite API
  slug: depict-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-lite-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Depictai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Depict.AI secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Depict.AI
provider_slug: depictai
scheme_count: 5
schemes:
- flows:
  - authorizationUrl: https://depict.eu.auth0.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://depict.eu.auth0.com/oauth/token
  name: Auth0
  sources:
  - openapi/depictai-lite-openapi.json
  - openapi/depictai-portal-openapi.json
  type: oauth2
- in: query
  name: APIKeyQuery
  parameter: api_key
  sources:
  - openapi/depictai-storefront-openapi.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/depictai-storefront-openapi.json
  type: apiKey
- in: cookie
  name: APIKeyCookie
  parameter: X-API-KEY
  sources:
  - openapi/depictai-storefront-openapi.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/depictai-storefront-openapi.json
  type: http
slug: depictai-authentication
source_filename: depictai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/depictai-lite-openapi.json, openapi/depictai-portal-openapi.json, openapi/depictai-storefront-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Auth0\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://depict.eu.auth0.com/oauth/authorize\n    tokenUrl: https://depict.eu.auth0.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/depictai-lite-openapi.json\n  - openapi/depictai-portal-openapi.json\n- name: APIKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/depictai-storefront-openapi.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/depictai-storefront-openapi.json\n- name: APIKeyCookie\n  type: apiKey\n  in: cookie\n  parameter: X-API-KEY\n  sources:\n  - openapi/depictai-storefront-openapi.json\n\
  - name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/depictai-storefront-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/authentication/depictai-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- E Commerce
- Search
- Recommendations
- Merchandising
- Personalization
- Product Discovery
- Retail
- Shopify
- Artificial Intelligence
---
