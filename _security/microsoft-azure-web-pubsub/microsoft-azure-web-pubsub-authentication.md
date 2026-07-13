---
api_key_in: []
api_specs:
- filename: webpubsub.json
  format: json
  label: Azure Web PubSub Service REST API
  slug: azure-web-pubsub-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/data-plane/WebPubSub/stable/2024-01-01/webpubsub.json
- filename: microsoft-azure-web-pubsub-asyncapi.yml
  format: yaml
  label: Azure Web PubSub Client and Upstream Events
  slug: azure-web-pubsub-client-and-upstream-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/main/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml
- filename: webpubsub.json
  format: json
  label: Azure Web PubSub Management REST API
  slug: azure-web-pubsub-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/resource-manager/Microsoft.SignalRService/stable/2024-03-01/webpubsub.json
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
