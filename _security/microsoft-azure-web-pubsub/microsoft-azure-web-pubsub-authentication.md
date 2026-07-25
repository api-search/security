---
api_key_in: []
api_specs:
- filename: microsoft-azure-web-pubsub-asyncapi.yml
  format: yaml
  label: Azure Web PubSub Client and Upstream Events
  slug: azure-web-pubsub-client-and-upstream-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/main/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml
- filename: microsoft-azure-web-pubsub-clienttoken-api-openapi.yml
  format: yaml
  label: Azure Web PubSub ClientToken API
  slug: microsoft-azure-web-pubsub-clienttoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/openapi/microsoft-azure-web-pubsub-clienttoken-api-openapi.yml
- filename: microsoft-azure-web-pubsub-hub-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Hub API
  slug: microsoft-azure-web-pubsub-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/openapi/microsoft-azure-web-pubsub-hub-api-openapi.yml
- filename: microsoft-azure-web-pubsub-permission-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Permission API
  slug: microsoft-azure-web-pubsub-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/openapi/microsoft-azure-web-pubsub-permission-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Web Pubsub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Web PubSub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Web PubSub
provider_slug: microsoft-azure-web-pubsub
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT signed with the service AccessKey using HS256, or a Microsoft

    Entra ID OAuth 2.0 bearer token with scope

    https://webpubsub.azure.com/.default'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-web-pubsub-openapi.yml
  type: http
slug: microsoft-azure-web-pubsub-authentication
source_filename: microsoft-azure-web-pubsub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-web-pubsub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT signed with the service AccessKey using HS256, or a Microsoft\n    Entra ID OAuth 2.0 bearer token with scope\n    https://webpubsub.azure.com/.default\n  sources:\n  - openapi/microsoft-azure-web-pubsub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/authentication/microsoft-azure-web-pubsub-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- Pub-Sub
- Real-Time
- Serverless
- WebSockets
---
