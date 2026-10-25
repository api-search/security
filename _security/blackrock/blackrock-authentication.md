---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: blackrock-authorizationurl-generate-api-openapi.yml
  format: yaml
  label: BlackRock Authorization Url:generate API
  slug: blackrock-authorizationurl-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-authorizationurl-generate-api-openapi.yml
- filename: blackrock-studionotifications-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications API
  slug: blackrock-studionotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-api-openapi.yml
- filename: blackrock-studionotifications-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:batch Create API
  slug: blackrock-studionotifications-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-batchcreate-api-openapi.yml
- filename: blackrock-studionotifications-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:filter API
  slug: blackrock-studionotifications-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-filter-api-openapi.yml
- filename: blackrock-studiosubscriptions-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions API
  slug: blackrock-studiosubscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-api-openapi.yml
- filename: blackrock-studiosubscriptions-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:batch Create API
  slug: blackrock-studiosubscriptions-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-batchcreate-api-openapi.yml
- filename: blackrock-studiosubscriptions-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:filter API
  slug: blackrock-studiosubscriptions-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-filter-api-openapi.yml
- filename: blackrock-token-checktokenexists-api-openapi.yml
  format: yaml
  label: BlackRock Token:check Token Exists API
  slug: blackrock-token-checktokenexists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-checktokenexists-api-openapi.yml
- filename: blackrock-token-generate-api-openapi.yml
  format: yaml
  label: BlackRock Token:generate API
  slug: blackrock-token-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-generate-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Blackrock Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: BlackRock secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: BlackRock
provider_slug: blackrock
scheme_count: 5
schemes:
- in: header
  name: APIKeyHeader
  parameter: VND.com.blackrock.API-Key
  sources:
  - openapi/blackrock-studio-notification-openapi.yml
  - openapi/blackrock-studio-subscription-openapi.yml
  - openapi/blackrock-token-openapi.yml
  type: apiKey
- in: header
  name: ClientKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/blackrock-studio-notification-openapi.yml
  - openapi/blackrock-studio-subscription-openapi.yml
  - openapi/blackrock-token-openapi.yml
  type: apiKey
- description: This API uses OAuth 2.0 with the access code flow.
  flows:
  - authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2AccessCode
  sources:
  - openapi/blackrock-studio-notification-openapi.yml
  - openapi/blackrock-studio-subscription-openapi.yml
  - openapi/blackrock-token-openapi.yml
  type: oauth2
- description: This API uses OAuth 2.0 with the client credentials flow.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/blackrock-studio-notification-openapi.yml
  - openapi/blackrock-studio-subscription-openapi.yml
  - openapi/blackrock-token-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/blackrock-studio-notification-openapi.yml
  - openapi/blackrock-studio-subscription-openapi.yml
  - openapi/blackrock-token-openapi.yml
  type: http
slug: blackrock-authentication
source_filename: blackrock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/blackrock-studio-notification-openapi.yml, openapi/blackrock-studio-subscription-openapi.yml,\n  openapi/blackrock-token-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: VND.com.blackrock.API-Key\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n- name: ClientKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n- name: OAuth2AccessCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize\n\
  \    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n    scopes: 2\n  description: This API uses OAuth 2.0 with the access code flow.\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n    scopes: 2\n  description: This API uses OAuth 2.0 with the client credentials flow.\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/authentication/blackrock-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Asset Management
- Finance
- Fintech
- Investment Management
- Portfolio Management
- Risk Analytics
- Fortune 500
---
