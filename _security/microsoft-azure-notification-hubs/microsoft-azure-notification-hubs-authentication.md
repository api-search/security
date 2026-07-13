---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-notification-hubs-openapi.yml
  format: yaml
  label: Azure Notification Hubs REST API
  slug: azure-notification-hubs-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-notification-hubs/refs/heads/main/openapi/microsoft-azure-notification-hubs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Notification Hubs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Notification Hubs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Notification Hubs
provider_slug: microsoft-azure-notification-hubs
scheme_count: 1
schemes:
- in: header
  name: sasToken
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-notification-hubs-openapi.yml
  type: apiKey
slug: microsoft-azure-notification-hubs-authentication
source_filename: microsoft-azure-notification-hubs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-notification-hubs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sasToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/microsoft-azure-notification-hubs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-notification-hubs/refs/heads/main/authentication/microsoft-azure-notification-hubs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cross-Platform
- Messaging
- Mobile
- Notifications
- Push Notifications
---
