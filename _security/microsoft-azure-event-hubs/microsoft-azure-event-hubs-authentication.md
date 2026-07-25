---
api_key_in:
- header
api_specs:
- filename: azure-event-hubs-messaging-asyncapi.yml
  format: yaml
  label: Azure Event Hubs Messaging API
  slug: azure-event-hubs-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/asyncapi/azure-event-hubs-messaging-asyncapi.yml
- filename: microsoft-azure-event-hubs-authorization-rules-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Authorization Rules API
  slug: microsoft-azure-event-hubs-authorization-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-authorization-rules-api-openapi.yml
- filename: microsoft-azure-event-hubs-consumer-groups-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Consumer Groups API
  slug: microsoft-azure-event-hubs-consumer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-consumer-groups-api-openapi.yml
- filename: microsoft-azure-event-hubs-disaster-recovery-configs-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Disaster Recovery Configs API
  slug: microsoft-azure-event-hubs-disaster-recovery-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-disaster-recovery-configs-api-openapi.yml
- filename: microsoft-azure-event-hubs-event-hubs-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Event Hubs API
  slug: microsoft-azure-event-hubs-event-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-event-hubs-api-openapi.yml
- filename: microsoft-azure-event-hubs-events-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Events API
  slug: microsoft-azure-event-hubs-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-events-api-openapi.yml
- filename: microsoft-azure-event-hubs-namespaces-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Namespaces API
  slug: microsoft-azure-event-hubs-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-namespaces-api-openapi.yml
- filename: microsoft-azure-event-hubs-operations-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Operations API
  slug: microsoft-azure-event-hubs-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-operations-api-openapi.yml
- filename: microsoft-azure-event-hubs-schema-registry-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Schema Registry API
  slug: microsoft-azure-event-hubs-schema-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/openapi/microsoft-azure-event-hubs-schema-registry-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Event Hubs Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Event Hubs secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Event Hubs
provider_slug: microsoft-azure-event-hubs
scheme_count: 3
schemes:
- description: 'Shared Access Signature token. Format: SharedAccessSignature sr={namespace}.servicebus.windows.net&sig={signature}&se={expiry}&skn={keyName}'
  in: header
  name: sas_token
  parameter: Authorization
  sources:
  - openapi/azure-event-hubs-data-plane-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Azure Active Directory (Azure AD) JSON Web Token (JWT). Format: Bearer {Azure AD JWT token}'
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/azure-event-hubs-data-plane-openapi.yml
  type: http
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-event-hubs-management-openapi.yml
  type: oauth2
slug: microsoft-azure-event-hubs-authentication
source_filename: microsoft-azure-event-hubs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-event-hubs-data-plane-openapi.yml, openapi/azure-event-hubs-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: sas_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Shared Access Signature token. Format: SharedAccessSignature sr={namespace}.servicebus.windows.net&sig={signature}&se={expiry}&skn={keyName}'\n  sources:\n  - openapi/azure-event-hubs-data-plane-openapi.yml\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Azure Active Directory (Azure AD) JSON Web Token (JWT). Format: Bearer {Azure\n    AD JWT token}'\n  sources:\n  - openapi/azure-event-hubs-data-plane-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n\
  \  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-event-hubs-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/authentication/microsoft-azure-event-hubs-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Big Data
- Event Streaming
- IoT
- Message Ingestion
- Real-Time Processing
---
