---
api_key_in:
- header
api_specs:
- filename: azure-event-grid-openapi.yml
  format: yaml
  label: Azure Event Grid Publisher API
  slug: publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-event-grid/refs/heads/main/openapi/azure-event-grid-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Event Grid Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azure Event Grid secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azure Event Grid
provider_slug: azure-event-grid
scheme_count: 3
schemes:
- description: Topic shared-access key
  in: header
  name: sasKey
  parameter: aeg-sas-key
  sources:
  - openapi/azure-event-grid-openapi.yml
  type: apiKey
- description: Topic shared-access signature token
  in: header
  name: sasToken
  parameter: aeg-sas-token
  sources:
  - openapi/azure-event-grid-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-event-grid-openapi.yml
  type: oauth2
slug: azure-event-grid-authentication
source_filename: azure-event-grid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-event-grid-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: sasKey\n  type: apiKey\n  in: header\n  parameter: aeg-sas-key\n  description: Topic shared-access key\n  sources:\n  - openapi/azure-event-grid-openapi.yml\n- name: sasToken\n  type: apiKey\n  in: header\n  parameter: aeg-sas-token\n  description: Topic shared-access signature token\n  sources:\n  - openapi/azure-event-grid-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n  sources:\n  - openapi/azure-event-grid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-event-grid/refs/heads/main/authentication/azure-event-grid-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Eventing
- Event Driven
- Pub Sub
- Messaging
- Webhooks
- CloudEvents
- Cloud
- Azure
---
