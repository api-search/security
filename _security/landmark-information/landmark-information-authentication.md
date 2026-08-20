---
api_key_in:
- header
api_specs:
- filename: landmark-information-order-experience-api-openapi.yml
  format: yaml
  label: Landmark Order Experience API
  slug: landmark-order-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-order-experience-api-openapi.yml
- filename: landmark-information-conveyancing-experience-api-openapi.yml
  format: yaml
  label: Landmark Conveyancing Experience API
  slug: landmark-conveyancing-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-conveyancing-experience-api-openapi.yml
- filename: landmark-information-intelliworks-api-openapi.yml
  format: yaml
  label: Landmark Intelliworks APIs
  slug: landmark-intelliworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-intelliworks-api-openapi.yml
- filename: landmark-information-document-vault-api-openapi.yml
  format: yaml
  label: Landmark Document Vault API
  slug: landmark-document-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-document-vault-api-openapi.yml
- filename: landmark-information-milestone-notification-service-api-openapi.yml
  format: yaml
  label: Landmark Milestone Notification Service API
  slug: landmark-milestone-notification-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-milestone-notification-service-api-openapi.yml
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Landmark Information Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Landmark Information Group secures its APIs with http, oauth2, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Landmark Information Group
provider_slug: landmark-information
scheme_count: 3
schemes:
- description: 'OAuth 2.0 client credentials. Request an access token from the token endpoint for your

    environment, then send it as a bearer token on every request. See **Authentication** for details.'
  flows:
  - flow: clientCredentials
    note: the spec declares an empty scopes map; Landmark documents no scope surface
    scopes: 0
    tokenUrl: https://lmkmaster.eu.auth0.com/oauth/token
  name: BearerAuth
  sources:
  - openapi/landmark-information-conveyancing-experience-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  note: Declared as plain HTTP bearer in four of the five specs, but the documented way to obtain the token is the same Auth0 client-credentials exchange as BearerAuth above.
  scheme: bearer
  sources:
  - openapi/landmark-information-document-vault-api-openapi.yml
  - openapi/landmark-information-intelliworks-api-openapi.yml
  - openapi/landmark-information-milestone-notification-service-api-openapi.yml
  - openapi/landmark-information-order-experience-api-openapi.yml
  type: http
- in: header
  name: x-api-key
  note: Planning API (powered by Barbour ABI) only. Documented in public HTML, not in an OpenAPI. A Landmark-issued API key is sent alongside a Basic-auth login call (base64 of username and a SHA256-hashed password) that returns a bearer token valid until 30 days of disuse.
  parameter: x-api-key
  sources:
  - https://www.landmark.co.uk/products/planning-api/planning-api-documentation/
  type: apiKey
slug: landmark-information-authentication
source_filename: landmark-information-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/landmark-information-conveyancing-experience-api-openapi.yml, openapi/landmark-information-document-vault-api-openapi.yml,\n  openapi/landmark-information-intelliworks-api-openapi.yml, openapi/landmark-information-milestone-notification-service-api-openapi.yml,\n  openapi/landmark-information-order-experience-api-openapi.yml\ndocs: https://www.landmarkcloudservices.com/?api=document-vault-experience\ndiscovery: authentication/landmark-information-openid-configuration.json\nsummary:\n  types:\n  - http\n  - oauth2\n  - apiKey\n  oauth2_flows:\n  - clientCredentials\n  api_key_in:\n  - header\n  model: >-\n    Every API on the Landmark Cloud Services platform is OAuth 2.0 client credentials against\n    Landmark's Auth0 tenant. Client ID and secret are issued only after commercial onboarding, and\n    separately per environment - UAT and production are different credentials against different\n    Auth0 tenants. The access\
  \ token is a JWT sent as Authorization: Bearer on every call, and the\n    audience parameter is fixed per environment and must be supplied on the token request. Some\n    APIs additionally require an Account-Id header identifying the onboarded firm. The Planning API\n    is the exception: it sits on a different host (api.barbour-abi.com) and uses a Landmark-issued\n    x-api-key plus a Basic-auth login exchange rather than OAuth.\n  identity_provider: Auth0 (lmkmaster.eu.auth0.com / lmkmaster-uat.eu.auth0.com)\n  onboarding: partner-only; credentials issued by a Landmark commercial contact\nenvironments:\n- name: production\n  token_url: https://lmkmaster.eu.auth0.com/oauth/token\n  audience: https://api.landmarkcloudservices.com\n  api_base: https://api.landmarkcloudservices.com\n- name: uat\n  token_url: https://lmkmaster-uat.eu.auth0.com/oauth/token\n  audience: https://uat-api.landmarkcloudservices.com\n  api_base: https://uat-api.landmarkcloudservices.com\nschemes:\n- name: BearerAuth\n\
  \  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://lmkmaster.eu.auth0.com/oauth/token\n    scopes: 0\n    note: the spec declares an empty scopes map; Landmark documents no scope surface\n  description: |-\n    OAuth 2.0 client credentials. Request an access token from the token endpoint for your\n    environment, then send it as a bearer token on every request. See **Authentication** for details.\n  sources:\n  - openapi/landmark-information-conveyancing-experience-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: >-\n    Declared as plain HTTP bearer in four of the five specs, but the documented way to obtain the\n    token is the same Auth0 client-credentials exchange as BearerAuth above.\n  sources:\n  - openapi/landmark-information-document-vault-api-openapi.yml\n  - openapi/landmark-information-intelliworks-api-openapi.yml\n  - openapi/landmark-information-milestone-notification-service-api-openapi.yml\n \
  \ - openapi/landmark-information-order-experience-api-openapi.yml\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  note: >-\n    Planning API (powered by Barbour ABI) only. Documented in public HTML, not in an OpenAPI. A\n    Landmark-issued API key is sent alongside a Basic-auth login call (base64 of username and a\n    SHA256-hashed password) that returns a bearer token valid until 30 days of disuse.\n  sources:\n  - https://www.landmark.co.uk/products/planning-api/planning-api-documentation/\nadditional_headers:\n- name: Account-Id\n  required_by:\n  - Document Vault API\n  description: The onboarded account identifier issued with the credentials; sent on every request.\n- name: Authorization\n  required_by:\n  - all Landmark Cloud Services APIs\n  description: Bearer <access_token>\ncallback_authentication:\n  description: >-\n    Landmark calls consumer-hosted callback URLs for milestone notifications, and authenticates\n    outbound to them using one of\
  \ three mechanisms configured at registration time.\n  mechanisms:\n  - Basic\n  - ClientIdSecret\n  - OAuth2 client credentials against a consumer-supplied token_generation_url, with optional\n    audience and scope\n  source: openapi/landmark-information-milestone-notification-service-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/authentication/landmark-information-authentication.yml
summary_line: http/oauth2/apiKey · 3 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Conveyancing
- Land Registry
- Geospatial
- Valuation
- Anti-Money Laundering
- Planning Data
- Mortgage
---
