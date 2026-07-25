---
api_key_in: []
api_specs:
- filename: zubale-api-documentation-for-external-notification-handler-api-openapi.yml
  format: yaml
  label: Zubale API Documentation for External Notification Handler API
  slug: zubale-api-documentation-for-external-notification-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-api-documentation-for-external-notification-handler-api-openapi.yml
- filename: zubale-cancel-tasks-api-openapi.yml
  format: yaml
  label: Zubale Cancel tasks API
  slug: zubale-cancel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-cancel-tasks-api-openapi.yml
- filename: zubale-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Delivery API API
  slug: zubale-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-delivery-api-api-openapi.yml
- filename: zubale-external-outbound-api-openapi.yml
  format: yaml
  label: Zubale External outbound API
  slug: zubale-external-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-external-outbound-api-openapi.yml
- filename: zubale-live-tracking-for-cencosud-api-openapi.yml
  format: yaml
  label: Zubale Live Tracking For Cencosud API
  slug: zubale-live-tracking-for-cencosud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-live-tracking-for-cencosud-api-openapi.yml
- filename: zubale-picking-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Picking & Delivery API API
  slug: zubale-picking-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-picking-delivery-api-api-openapi.yml
- filename: zubale-product-catalog-api-openapi.yml
  format: yaml
  label: Zubale Product catalog API
  slug: zubale-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-product-catalog-api-openapi.yml
- filename: zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
  format: yaml
  label: 'Zubale Webhook: Payload Structure for Order Notification API'
  slug: zubale-webhook-payload-structure-for-order-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zubale Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zubale secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zubale
provider_slug: zubale
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'OAuth2 client-credentials access token from POST /oauth2/token, sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zubale-openapi.yml
  type: http
- description: HTTP Basic (client_id:client_secret) used only against POST /oauth2/token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/zubale-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.zubale.com/oauth2/token
  name: oauth2
  sources:
  - openapi/zubale-openapi.yml
  type: oauth2
slug: zubale-authentication
source_filename: zubale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zubale-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 client-credentials access token from POST /oauth2/token, sent as Authorization:\n    Bearer <token>.'\n  sources:\n  - openapi/zubale-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic (client_id:client_secret) used only against POST /oauth2/token.\n  sources:\n  - openapi/zubale-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zubale.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/zubale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/authentication/zubale-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Ecommerce
---
