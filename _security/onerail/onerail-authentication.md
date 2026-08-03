---
api_key_in:
- header
api_specs:
- filename: onerail-delivery-api-openapi.yml
  format: yaml
  label: OneRail Delivery API
  slug: onerail-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-delivery-api-openapi.yml
- filename: onerail-operations-api-openapi.yml
  format: yaml
  label: OneRail Operations API
  slug: onerail-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-operations-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Onerail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OneRail secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OneRail
provider_slug: onerail
scheme_count: 5
schemes:
- in: header
  name: ApiKey
  parameter: X-ONERAIL-API-KEY
  sources:
  - openapi/onerail-delivery-api-openapi.yml
  - openapi/onerail-operations-api-openapi.yml
  type: apiKey
- in: header
  name: AppId
  parameter: X-ONERAIL-APP-ID
  sources:
  - openapi/onerail-delivery-api-openapi.yml
  - openapi/onerail-operations-api-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAndAppId
  parameter: X-ONERAIL-API-KEY-AND-APP-ID
  sources:
  - openapi/onerail-delivery-api-openapi.yml
  type: apiKey
- description: 'Standard JWT bearer token used for authenticated OmniPoint users

    and internal service-to-service calls. Clients send `Authorization: Bearer <jwt>`

    and the token is validated using the shared Core access token secret.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/onerail-operations-api-openapi.yml
  type: http
- description: 'OAuth 2.0 access token validated by the Operations service (e.g. Okta-backed

    integrations). Clients obtain tokens from their own IdP outside of this API

    and call endpoints with `Authorization: OAuth <access_token>`. The

    `authorizationUrl` and `tokenUrl` values below are placeholders only to

    satisfy the OpenAPI schema; this service does not call them directly and the

    real IdP URLs are configured vi'
  flows:
  - authorizationUrl: https://dummy-unused-url.com
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://dummy-unused-url.com
  name: OAuth
  sources:
  - openapi/onerail-operations-api-openapi.yml
  type: oauth2
slug: onerail-authentication
source_filename: onerail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/onerail-delivery-api-openapi.yml, openapi/onerail-operations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-ONERAIL-API-KEY\n  sources:\n  - openapi/onerail-delivery-api-openapi.yml\n  - openapi/onerail-operations-api-openapi.yml\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: X-ONERAIL-APP-ID\n  sources:\n  - openapi/onerail-delivery-api-openapi.yml\n  - openapi/onerail-operations-api-openapi.yml\n- name: ApiKeyAndAppId\n  type: apiKey\n  in: header\n  parameter: X-ONERAIL-API-KEY-AND-APP-ID\n  sources:\n  - openapi/onerail-delivery-api-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  description: |-\n    Standard JWT bearer token used for authenticated OmniPoint users\n    and internal service-to-service calls. Clients send `Authorization:\
  \ Bearer <jwt>`\n    and the token is validated using the shared Core access token secret.\n  sources:\n  - openapi/onerail-operations-api-openapi.yml\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dummy-unused-url.com\n    tokenUrl: https://dummy-unused-url.com\n    scopes: 0\n  description: |-\n    OAuth 2.0 access token validated by the Operations service (e.g. Okta-backed\n    integrations). Clients obtain tokens from their own IdP outside of this API\n    and call endpoints with `Authorization: OAuth <access_token>`. The\n    `authorizationUrl` and `tokenUrl` values below are placeholders only to\n    satisfy the OpenAPI schema; this service does not call them directly and the\n    real IdP URLs are configured vi\n  sources:\n  - openapi/onerail-operations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/authentication/onerail-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- last-mile-delivery
- delivery-orchestration
- logistics
- supply-chain
- route-optimization
- courier-network
- shipping
- fleet-management
- transportation
- order-management
- webhooks
- final-mile
---
