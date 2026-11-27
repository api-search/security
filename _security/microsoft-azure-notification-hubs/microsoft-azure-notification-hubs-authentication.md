---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-azure-notification-hubs-hubs-api-openapi.yml
  format: yaml
  label: Azure Notification Hubs Hubs API
  slug: microsoft-azure-notification-hubs-hubs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-notification-hubs/openapi/microsoft-azure-notification-hubs-hubs-api-openapi.yml
- filename: microsoft-azure-notification-hubs-namespaces-api-openapi.yml
  format: yaml
  label: Azure Notification Hubs Namespaces API
  slug: microsoft-azure-notification-hubs-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-notification-hubs/openapi/microsoft-azure-notification-hubs-namespaces-api-openapi.yml
- filename: microsoft-azure-notification-hubs-operations-api-openapi.yml
  format: yaml
  label: Azure Notification Hubs Operations API
  slug: microsoft-azure-notification-hubs-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-notification-hubs/openapi/microsoft-azure-notification-hubs-operations-api-openapi.yml
- filename: microsoft-azure-notification-hubs-private-link-api-openapi.yml
  format: yaml
  label: Azure Notification Hubs Private Link API
  slug: microsoft-azure-notification-hubs-private-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-notification-hubs/openapi/microsoft-azure-notification-hubs-private-link-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Azure Notification Hubs Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Notification Hubs secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Notification Hubs
provider_slug: microsoft-azure-notification-hubs
scheme_count: 2
schemes:
- in: header
  name: sasToken
  parameter: Authorization
  sources:
  - openapi/_superseded/microsoft-azure-notification-hubs-installations-api-openapi.yml
  - openapi/_superseded/microsoft-azure-notification-hubs-notifications-api-openapi.yml
  - openapi/_superseded/microsoft-azure-notification-hubs-registrations-api-openapi.yml
  type: apiKey
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-notification-hubs-resource-manager-openapi.yml
  type: oauth2
slug: microsoft-azure-notification-hubs-authentication
source_filename: microsoft-azure-notification-hubs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-notification-hubs-installations-api-openapi.yml, openapi/_superseded/microsoft-azure-notification-hubs-notifications-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-notification-hubs-registrations-api-openapi.yml, openapi/microsoft-azure-notification-hubs-resource-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: sasToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/_superseded/microsoft-azure-notification-hubs-installations-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-notification-hubs-notifications-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-notification-hubs-registrations-api-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/microsoft-azure-notification-hubs-resource-manager-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-notification-hubs/authentication/microsoft-azure-notification-hubs-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Cross-Platform
- Messaging
- Mobile
- Notification
- Push Notifications
---
