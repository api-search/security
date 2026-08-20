---
api_key_in:
- header
api_specs:
- filename: decisiv-account-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Account Management
  slug: decisiv-srm-gateway-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-account-management-openapi.yml
- filename: decisiv-asset-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Asset Management
  slug: decisiv-srm-gateway-asset-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-asset-management-openapi.yml
- filename: decisiv-service-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Service Management
  slug: decisiv-srm-gateway-service-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-management-openapi.yml
- filename: decisiv-telematics-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Telematics
  slug: decisiv-srm-gateway-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-telematics-openapi.yml
- filename: decisiv-global-assets-openapi.yml
  format: yaml
  label: Decisiv Global Assets API
  slug: decisiv-global-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-global-assets-openapi.yml
- filename: decisiv-service-provider-openapi.yml
  format: yaml
  label: Decisiv Service Provider API
  slug: decisiv-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-provider-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Decisiv Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Decisiv secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Decisiv
provider_slug: decisiv
scheme_count: 5
schemes:
- bearerFormat: JWT
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/decisiv-account-management-openapi.yml
  - openapi/decisiv-asset-management-openapi.yml
  - openapi/decisiv-service-management-openapi.yml
  - openapi/decisiv-telematics-openapi.yml
  type: http
- description: OAuth 2.0 Authorization Code flow. This is the required flow for new integrations. See https://api-docs.decisiv.net/docs/api/oauth/
  flows:
  - authorizationUrl: https://login.decisiv.net/auth/api_gateway
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://login.decisiv.net/oauth/token
  name: OAuth2AuthorizationCode
  sources:
  - openapi/decisiv-account-management-openapi.yml
  - openapi/decisiv-asset-management-openapi.yml
  - openapi/decisiv-service-management-openapi.yml
  - openapi/decisiv-telematics-openapi.yml
  type: oauth2
- description: '**Deprecated.** OAuth 2.0 Password flow. New integrations must use the Authorization Code flow (`OAuth2AuthorizationCode`); this flow remains available only during the migration window and will be removed in a future release. See https://api-docs.decisiv.net/docs/api/oauth/'
  flows:
  - flow: password
    scopes: 0
    tokenUrl: https://login.decisiv.net/oauth/token
  name: OAuth2Password
  sources:
  - openapi/decisiv-account-management-openapi.yml
  - openapi/decisiv-asset-management-openapi.yml
  - openapi/decisiv-global-assets-openapi.yml
  - openapi/decisiv-service-management-openapi.yml
  - openapi/decisiv-service-provider-openapi.yml
  - openapi/decisiv-telematics-openapi.yml
  type: oauth2
- description: The transition token must be specified when using OAuth. Please see https://api-docs.decisiv.net/docs/api/oauth/
  in: header
  name: TransitionToken
  parameter: X-Decisiv-Transition-Token
  sources:
  - openapi/decisiv-global-assets-openapi.yml
  - openapi/decisiv-service-provider-openapi.yml
  type: apiKey
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/decisiv-global-assets-openapi.yml
  - openapi/decisiv-service-provider-openapi.yml
  type: apiKey
slug: decisiv-authentication
source_filename: decisiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/decisiv-account-management-openapi.yml, openapi/decisiv-asset-management-openapi.yml,\n  openapi/decisiv-global-assets-openapi.yml, openapi/decisiv-service-management-openapi.yml,\n  openapi/decisiv-service-provider-openapi.yml, openapi/decisiv-telematics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/decisiv-account-management-openapi.yml\n  - openapi/decisiv-asset-management-openapi.yml\n  - openapi/decisiv-service-management-openapi.yml\n  - openapi/decisiv-telematics-openapi.yml\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.decisiv.net/auth/api_gateway\n    tokenUrl: https://login.decisiv.net/oauth/token\n    scopes: 0\n  description:\
  \ OAuth 2.0 Authorization Code flow. This is the required flow for new integrations.\n    See https://api-docs.decisiv.net/docs/api/oauth/\n  sources:\n  - openapi/decisiv-account-management-openapi.yml\n  - openapi/decisiv-asset-management-openapi.yml\n  - openapi/decisiv-service-management-openapi.yml\n  - openapi/decisiv-telematics-openapi.yml\n- name: OAuth2Password\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://login.decisiv.net/oauth/token\n    scopes: 0\n  description: '**Deprecated.** OAuth 2.0 Password flow. New integrations must use the Authorization\n    Code flow (`OAuth2AuthorizationCode`); this flow remains available only during the migration\n    window and will be removed in a future release. See https://api-docs.decisiv.net/docs/api/oauth/'\n  sources:\n  - openapi/decisiv-account-management-openapi.yml\n  - openapi/decisiv-asset-management-openapi.yml\n  - openapi/decisiv-global-assets-openapi.yml\n  - openapi/decisiv-service-management-openapi.yml\n\
  \  - openapi/decisiv-service-provider-openapi.yml\n  - openapi/decisiv-telematics-openapi.yml\n- name: TransitionToken\n  type: apiKey\n  in: header\n  parameter: X-Decisiv-Transition-Token\n  description: The transition token must be specified when using OAuth. Please see https://api-docs.decisiv.net/docs/api/oauth/\n  sources:\n  - openapi/decisiv-global-assets-openapi.yml\n  - openapi/decisiv-service-provider-openapi.yml\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/decisiv-global-assets-openapi.yml\n  - openapi/decisiv-service-provider-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/authentication/decisiv-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- commercial-vehicle
- Fleet Management
- service-relationship-management
- Telematics
- Asset Management
- maintenance-and-repair
- Heavy Duty Trucking
- Transportation
- Dealer Management
- JSON:API
- Webhook
---
