---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-blob-storage-azure-storage-blob-service-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Azure Storage Blob Service API
  slug: microsoft-azure-blob-storage-azure-storage-blob-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-azure-storage-blob-service-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Azure Blob Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Blob Storage secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure Blob Storage
provider_slug: microsoft-azure-blob-storage
scheme_count: 3
schemes:
- description: Azure Storage shared key authorization using the storage account access key.
  in: header
  name: sharedKey
  parameter: Authorization
  sources:
  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: http
- description: Shared access signature (SAS) token granting delegated access to blob resources.
  in: query
  name: sharedAccessSignature
  parameter: sig
  sources:
  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: apiKey
slug: microsoft-azure-blob-storage-authentication
source_filename: microsoft-azure-blob-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml, openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml, openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml, openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Azure Storage shared key authorization using the storage account access key.\n  sources:\n  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n \
  \ - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.\n  sources:\n  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n- name:\
  \ sharedAccessSignature\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared access signature (SAS) token granting delegated access to blob resources.\n  sources:\n  - openapi/_superseded/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-blob-storage/authentication/microsoft-azure-blob-storage-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Microsoft Azure
- Blobs
- Cloud Storage
- Microsoft
- Object Storage
- Storage
---
