---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-service-bus-openapi.yml
  format: yaml
  label: Azure Service Bus REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-service-bus/refs/heads/main/openapi/microsoft-azure-service-bus-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Service Bus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Service Bus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Service Bus
provider_slug: microsoft-azure-service-bus
scheme_count: 1
schemes:
- description: SAS token in Authorization header
  in: header
  name: sasToken
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-service-bus-openapi.yml
  type: apiKey
slug: microsoft-azure-service-bus-authentication
source_filename: microsoft-azure-service-bus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-service-bus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sasToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: SAS token in Authorization header\n  sources:\n  - openapi/microsoft-azure-service-bus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-service-bus/refs/heads/main/authentication/microsoft-azure-service-bus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Enterprise Messaging
- Message Broker
- Messaging
- Publish Subscribe
- Queues
- Topics
---
