---
api_key_in: []
api_specs:
- filename: microsoft-azure-signalr-openapi.yml
  format: yaml
  label: Azure SignalR Service REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-signalr/refs/heads/main/openapi/microsoft-azure-signalr-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Signalr Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure SignalR Service secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure SignalR Service
provider_slug: microsoft-azure-signalr
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-signalr-openapi.yml
  type: oauth2
slug: microsoft-azure-signalr-authentication
source_filename: microsoft-azure-signalr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-signalr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-signalr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-signalr/refs/heads/main/authentication/microsoft-azure-signalr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real-Time
- WebSockets
- SignalR
- Messaging
- Push
---
