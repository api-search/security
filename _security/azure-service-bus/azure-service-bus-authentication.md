---
api_key_in: []
api_specs:
- filename: azure-service-bus-openapi.yml
  format: yaml
  label: Azure Service Bus
  slug: azure-service-bus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-service-bus/refs/heads/main/openapi/azure-service-bus-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Service Bus Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Service Bus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Service Bus
provider_slug: azure-service-bus
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-service-bus-openapi.yml
  type: oauth2
slug: azure-service-bus-authentication
source_filename: azure-service-bus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-service-bus-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/azure-service-bus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-service-bus/refs/heads/main/authentication/azure-service-bus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cloud
- Enterprise
- Message Broker
- Messaging
- Pub/Sub
- Queues
---
