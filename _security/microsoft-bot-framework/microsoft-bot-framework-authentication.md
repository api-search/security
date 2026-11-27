---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-bot-framework-bot-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot API
  slug: microsoft-bot-framework-bot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bot-api-openapi.yml
- filename: microsoft-bot-framework-botconnection-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Connection API
  slug: microsoft-bot-framework-botconnection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-botconnection-api-openapi.yml
- filename: microsoft-bot-framework-bothostsettings-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Host Settings API
  slug: microsoft-bot-framework-bothostsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml
- filename: microsoft-bot-framework-channel-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Channel API
  slug: microsoft-bot-framework-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-channel-api-openapi.yml
- filename: microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Qn A Maker Endpoint Keys API
  slug: microsoft-bot-framework-listqnamakerendpointkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
- filename: microsoft-bot-framework-listserviceproviders-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Service Providers API
  slug: microsoft-bot-framework-listserviceproviders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml
- filename: microsoft-bot-framework-operationresults-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operation Results API
  slug: microsoft-bot-framework-operationresults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operationresults-api-openapi.yml
- filename: microsoft-bot-framework-operations-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operations API
  slug: microsoft-bot-framework-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operations-api-openapi.yml
- filename: microsoft-bot-framework-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Link Resources API
  slug: microsoft-bot-framework-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml
- filename: microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Endpoint Connections API
  slug: microsoft-bot-framework-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Microsoft Bot Framework Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bot Framework secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Microsoft Bot Framework
provider_slug: microsoft-bot-framework
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-bot-framework-activities-api-openapi.yml
  - openapi/_superseded/microsoft-bot-framework-attachments-api-openapi.yml
  - openapi/_superseded/microsoft-bot-framework-conversations-api-openapi.yml
  - openapi/_superseded/microsoft-bot-framework-members-api-openapi.yml
  type: http
- description: Access token to authenticate calls to the Bot Connector Service.
  in: header
  name: bearer_auth
  parameter: Authorization
  sources:
  - openapi/microsoft-bot-framework-connector-api-openapi.yml
  - openapi/microsoft-bot-framework-token-api-openapi.yml
  type: apiKey
slug: microsoft-bot-framework-authentication
source_filename: microsoft-bot-framework-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-bot-framework-activities-api-openapi.yml, openapi/_superseded/microsoft-bot-framework-attachments-api-openapi.yml,\n  openapi/microsoft-bot-framework-connector-api-openapi.yml, openapi/_superseded/microsoft-bot-framework-conversations-api-openapi.yml,\n  openapi/_superseded/microsoft-bot-framework-members-api-openapi.yml, openapi/microsoft-bot-framework-token-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_superseded/microsoft-bot-framework-activities-api-openapi.yml\n  - openapi/_superseded/microsoft-bot-framework-attachments-api-openapi.yml\n  - openapi/_superseded/microsoft-bot-framework-conversations-api-openapi.yml\n  - openapi/_superseded/microsoft-bot-framework-members-api-openapi.yml\n- name: bearer_auth\n  type: apiKey\n  in: header\n  parameter:\
  \ Authorization\n  description: Access token to authenticate calls to the Bot Connector Service.\n  sources:\n  - openapi/microsoft-bot-framework-connector-api-openapi.yml\n  - openapi/microsoft-bot-framework-token-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-bot-framework/authentication/microsoft-bot-framework-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Bots
- Conversational AI
- Messaging
- Bot Framework
- Direct Line
---
