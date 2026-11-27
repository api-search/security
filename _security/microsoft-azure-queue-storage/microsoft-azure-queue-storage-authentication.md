---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-azure-queue-storage-azure-queue-storage-api-openapi.yml
  format: yaml
  label: Azure Queue Storage Azure Queue Storage API
  slug: microsoft-azure-queue-storage-azure-queue-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-queue-storage/openapi/microsoft-azure-queue-storage-azure-queue-storage-api-openapi.yml
- filename: microsoft-azure-queue-storage-messages-api-openapi.yml
  format: yaml
  label: Azure Queue Storage Messages API
  slug: microsoft-azure-queue-storage-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-queue-storage/openapi/microsoft-azure-queue-storage-messages-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Azure Queue Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Queue Storage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Queue Storage
provider_slug: microsoft-azure-queue-storage
scheme_count: 1
schemes:
- in: header
  name: queue_shared_key
  parameter: Authorization
  sources:
  - openapi/_superseded/microsoft-azure-queue-storage-queues-api-openapi.yml
  type: apiKey
slug: microsoft-azure-queue-storage-authentication
source_filename: microsoft-azure-queue-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-queue-storage-queues-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: queue_shared_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/_superseded/microsoft-azure-queue-storage-queues-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-queue-storage/authentication/microsoft-azure-queue-storage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Asynchronous Processing
- Cloud Storage
- Messaging
- Queues
- Storage
---
