---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: azure-event-hubs-messaging-asyncapi.yml
  format: yaml
  label: Azure Event Hubs Messaging API
  slug: azure-event-hubs-messaging-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/asyncapi/azure-event-hubs-messaging-asyncapi.yml
- filename: microsoft-azure-event-hubs-operations-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Operations API
  slug: microsoft-azure-event-hubs-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-operations-api-openapi.yml
- filename: microsoft-azure-event-hubs-armdisasterrecoveries-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Arm Disaster Recoveries API
  slug: microsoft-azure-event-hubs-armdisasterrecoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-armdisasterrecoveries-api-openapi.yml
- filename: microsoft-azure-event-hubs-authorizationrules-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Authorization Rules API
  slug: microsoft-azure-event-hubs-authorizationrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-authorizationrules-api-openapi.yml
- filename: microsoft-azure-event-hubs-clusters-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Clusters API
  slug: microsoft-azure-event-hubs-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-clusters-api-openapi.yml
- filename: microsoft-azure-event-hubs-disasterrecoveryconfigs-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Disaster Recovery Configs API
  slug: microsoft-azure-event-hubs-disasterrecoveryconfigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-disasterrecoveryconfigs-api-openapi.yml
- filename: microsoft-azure-event-hubs-ehnamespaces-api-openapi.yml
  format: yaml
  label: Azure Event Hubs EH Namespaces API
  slug: microsoft-azure-event-hubs-ehnamespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-ehnamespaces-api-openapi.yml
- filename: microsoft-azure-event-hubs-eventhubs-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Event Hubs API
  slug: microsoft-azure-event-hubs-eventhubs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-eventhubs-api-openapi.yml
- filename: microsoft-azure-event-hubs-networkrulesets-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Network Rule Sets API
  slug: microsoft-azure-event-hubs-networkrulesets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-networkrulesets-api-openapi.yml
- filename: microsoft-azure-event-hubs-networksecurityperimeterconfigurations-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Network Security Perimeter Configurations API
  slug: microsoft-azure-event-hubs-networksecurityperimeterconfigurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-networksecurityperimeterconfigurations-api-openapi.yml
- filename: microsoft-azure-event-hubs-schemagroups-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Schema Groups API
  slug: microsoft-azure-event-hubs-schemagroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-schemagroups-api-openapi.yml
- filename: microsoft-azure-event-hubs-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Subscriptions API
  slug: microsoft-azure-event-hubs-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-subscriptions-api-openapi.yml
- filename: microsoft-azure-event-hubs-application-groups-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Application Groups API
  slug: microsoft-azure-event-hubs-application-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-application-groups-api-openapi.yml
- filename: microsoft-azure-event-hubs-consumer-groups-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Consumer Groups API
  slug: microsoft-azure-event-hubs-consumer-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-consumer-groups-api-openapi.yml
- filename: microsoft-azure-event-hubs-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Event Hubs Private Endpoint Connections API
  slug: microsoft-azure-event-hubs-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-event-hubs/openapi/microsoft-azure-event-hubs-private-endpoint-connections-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Azure Event Hubs Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Event Hubs secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Event Hubs
provider_slug: microsoft-azure-event-hubs
scheme_count: 3
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/_superseded/microsoft-azure-event-hubs-authorization-rules-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-consumer-groups-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-disaster-recovery-configs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-event-hubs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-namespaces-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-operations-api-openapi.yml
  - openapi/_superseded/microsoft-azure-event-hubs-schema-registry-api-openapi.yml
  type: oauth2
- description: 'Shared Access Signature token. Format: SharedAccessSignature sr={namespace}.servicebus.windows.net&sig={signature}&se={expiry}&skn={keyName}'
  in: header
  name: sas_token
  parameter: Authorization
  sources:
  - openapi/_superseded/microsoft-azure-event-hubs-events-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Azure Active Directory (Azure AD) JSON Web Token (JWT). Format: Bearer {Azure AD JWT token}'
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-azure-event-hubs-events-api-openapi.yml
  type: http
slug: microsoft-azure-event-hubs-authentication
source_filename: microsoft-azure-event-hubs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-event-hubs-authorization-rules-api-openapi.yml, openapi/_superseded/microsoft-azure-event-hubs-consumer-groups-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-event-hubs-disaster-recovery-configs-api-openapi.yml, openapi/_superseded/microsoft-azure-event-hubs-event-hubs-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-event-hubs-events-api-openapi.yml, openapi/_superseded/microsoft-azure-event-hubs-namespaces-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-event-hubs-operations-api-openapi.yml, openapi/_superseded/microsoft-azure-event-hubs-schema-registry-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description:\
  \ Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/_superseded/microsoft-azure-event-hubs-authorization-rules-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-consumer-groups-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-disaster-recovery-configs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-event-hubs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-namespaces-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-operations-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-event-hubs-schema-registry-api-openapi.yml\n- name: sas_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Shared Access Signature token. Format: SharedAccessSignature sr={namespace}.servicebus.windows.net&sig={signature}&se={expiry}&skn={keyName}'\n  sources:\n  - openapi/_superseded/microsoft-azure-event-hubs-events-api-openapi.yml\n- name: bearer_token\n  type: http\n  scheme:\
  \ bearer\n  bearerFormat: JWT\n  description: 'Azure Active Directory (Azure AD) JSON Web Token (JWT). Format: Bearer {Azure\n    AD JWT token}'\n  sources:\n  - openapi/_superseded/microsoft-azure-event-hubs-events-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-event-hubs/authentication/microsoft-azure-event-hubs-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Big Data
- Event Streaming
- IoT
- Message Ingestion
- Real-Time Processing
- Real-Time
---
