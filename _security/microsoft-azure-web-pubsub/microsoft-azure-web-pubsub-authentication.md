---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-web-pubsub-asyncapi.yml
  format: yaml
  label: Azure Web PubSub Client and Upstream Events
  slug: azure-web-pubsub-client-and-upstream-events
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml
- filename: microsoft-azure-web-pubsub-general-api-openapi.yml
  format: yaml
  label: Azure Web PubSub General API
  slug: microsoft-azure-web-pubsub-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-general-api-openapi.yml
- filename: microsoft-azure-web-pubsub-webpubsub-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Webpubsub API
  slug: microsoft-azure-web-pubsub-webpubsub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-webpubsub-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Azure Web PubSub Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Web PubSub secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Web PubSub
provider_slug: microsoft-azure-web-pubsub
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT signed with the service AccessKey using HS256, or a Microsoft

    Entra ID OAuth 2.0 bearer token with scope

    https://webpubsub.azure.com/.default'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-azure-web-pubsub-client-token-api-openapi.yml
  - openapi/_superseded/microsoft-azure-web-pubsub-hub-api-openapi.yml
  - openapi/_superseded/microsoft-azure-web-pubsub-permission-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml
  - openapi/microsoft-azure-web-pubsub-management-api-openapi.yml
  type: oauth2
slug: microsoft-azure-web-pubsub-authentication
source_filename: microsoft-azure-web-pubsub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-web-pubsub-client-token-api-openapi.yml, openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-web-pubsub-hub-api-openapi.yml, openapi/microsoft-azure-web-pubsub-management-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-web-pubsub-permission-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT signed with the service AccessKey using HS256, or a Microsoft\n    Entra ID OAuth 2.0 bearer token with scope\n    https://webpubsub.azure.com/.default\n  sources:\n  - openapi/_superseded/microsoft-azure-web-pubsub-client-token-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-web-pubsub-hub-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-web-pubsub-permission-api-openapi.yml\n- name:\
  \ OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml\n  - openapi/microsoft-azure-web-pubsub-management-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-web-pubsub/authentication/microsoft-azure-web-pubsub-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Messaging
- Pub/Sub
- Real-Time
- Serverless
- WebSocket
---
