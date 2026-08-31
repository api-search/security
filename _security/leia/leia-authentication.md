---
api_key_in:
- query
api_specs:
- filename: leia-media-transformation-api-openapi.yml
  format: yaml
  label: Leia Media Transformation API
  slug: leia-media-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-media-transformation-api-openapi.yml
- filename: leia-product-pricing-api-openapi.yml
  format: yaml
  label: Leia Product Pricing API
  slug: leia-product-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-product-pricing-api-openapi.yml
- filename: leia-protocol-api-openapi.yml
  format: yaml
  label: Leia Protocol API
  slug: leia-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-protocol-api-openapi.yml
- filename: leia-storage-api-openapi.yml
  format: yaml
  label: Leia Storage API
  slug: leia-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-storage-api-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Leia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Leia secures its APIs with oauth2, http, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Leia
provider_slug: leia
scheme_count: 2
schemes:
- applied_to: all Immersity Cloud API operations
  bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/leia-immersity-cloud-api-openapi.yml
  type: http
- in: query
  name: sec0
  note: Present in the published authentication OpenAPI document as a document-level default. The token endpoint itself is called with client_id/client_secret form parameters, not an api_key query string; treat this scheme as a documentation-platform default rather than a live requirement.
  parameter: api_key
  sources:
  - openapi/leia-immersity-authentication-openapi.yml
  type: apiKey
slug: leia-authentication
source_filename: leia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/leia-immersity-authentication-openapi.yml, openapi/leia-immersity-cloud-api-openapi.yml\ndocs: https://docs-api.immersity.ai/docs/getting-started\ndiscovery: well-known/leia-openid-configuration.json\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows:\n  - clientCredentials\n  primary: OAuth 2.0 client-credentials bearer token (JWT) issued by the Immersity Keycloak realm\nmodel: >-\n  Immersity AI uses the OAuth 2.0 client-credentials flow. A developer creates client ID / secret pairs on\n  the Immersity account page (Leia Account > Manage Account > API tab), POSTs them to the Keycloak realm\n  token endpoint with grant_type=client_credentials, and sends the returned JWT as\n  `Authorization: Bearer <access_token>` on every Immersity Cloud API call. There is no separate API-key\n  header; credentials must never be embedded in client code and should be rotated periodically\
  \ per the\n  provider's published guidance.\nissuer: https://auth.immersity.ai/auth/realms/immersity\nendpoints:\n  token: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token\n  authorization: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/auth\n  introspection: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token/introspect\n  userinfo: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/userinfo\n  jwks: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/certs\n  registration: https://auth.immersity.ai/auth/realms/immersity/clients-registrations/openid-connect\n  device_authorization: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/auth/device\n  pushed_authorization_request: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/ext/par/request\n  end_session: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/logout\n\
  \  account_management: https://auth.immersity.ai/auth/realms/immersity/account\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- implicit\n- password\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:uma-ticket\n- urn:openid:params:grant-type:ciba\ncode_challenge_methods_supported:\n- plain\n- S256\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: all Immersity Cloud API operations\n  sources:\n  - openapi/leia-immersity-cloud-api-openapi.yml\n- name: sec0\n  type: apiKey\n  in: query\n  parameter: api_key\n  note: >-\n    Present in the published authentication OpenAPI document as a document-level default. The token\n    endpoint itself is called with client_id/client_secret form parameters, not an api_key query string;\n    treat this scheme as a documentation-platform default rather than a live requirement.\n  sources:\n\
  \  - openapi/leia-immersity-authentication-openapi.yml\ncredential_management:\n  console: https://auth.immersity.ai/auth/realms/immersity/account\n  path: Leia Account > Manage Account > API tab > add Client ID / Secret Key pair\n  guidance:\n  - Store client credentials in encrypted storage or a secure key-management system\n  - Do not hard-code credentials in application code or config files\n  - Rotate client secrets periodically\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - https://docs-api.immersity.ai/docs/getting-started\n  - https://auth.immersity.ai/auth/realms/immersity/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/authentication/leia-authentication.yml
summary_line: oauth2/http/apiKey · 2 schemes
tags:
- 3D
- Spatial Computing
- Computer-Vision
- depth-estimation
- Image Processing
- Video Processing
- Generative AI
- Displays
- media-transformation
- Immersive Experiences
---
