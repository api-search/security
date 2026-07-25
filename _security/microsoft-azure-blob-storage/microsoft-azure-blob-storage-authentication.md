---
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Append Blobs API
  slug: microsoft-azure-blob-storage-append-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Azure Blob Storage REST API API
  slug: microsoft-azure-blob-storage-azure-blob-storage-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
- filename: microsoft-azure-blob-storage-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Blobs API
  slug: microsoft-azure-blob-storage-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Block Blobs API
  slug: microsoft-azure-blob-storage-block-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-comp-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?comp=blobs API
  slug: microsoft-azure-blob-storage-comp-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-comp-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-containers-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Containers API
  slug: microsoft-azure-blob-storage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
- filename: microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Page Blobs API
  slug: microsoft-azure-blob-storage-page-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-batch-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=batch API
  slug: microsoft-azure-blob-storage-restype-service-comp-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-batch-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-properties-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=properties API
  slug: microsoft-azure-blob-storage-restype-service-comp-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-properties-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-stats-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=stats API
  slug: microsoft-azure-blob-storage-restype-service-comp-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-stats-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=userdelegationkey API
  slug: microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Blob Storage Authentication
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
  - openapi/azure-blob-storage-rest-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/azure-blob-storage-rest-openapi.yml
  type: http
- description: Shared access signature (SAS) token granting delegated access to blob resources.
  in: query
  name: sharedAccessSignature
  parameter: sig
  sources:
  - openapi/azure-blob-storage-rest-openapi.yml
  type: apiKey
slug: microsoft-azure-blob-storage-authentication
source_filename: microsoft-azure-blob-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-blob-storage-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Azure Storage shared key authorization using the storage account access key.\n  sources:\n  - openapi/azure-blob-storage-rest-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.\n  sources:\n  - openapi/azure-blob-storage-rest-openapi.yml\n- name: sharedAccessSignature\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared access signature (SAS) token granting delegated access to blob resources.\n  sources:\n  - openapi/azure-blob-storage-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/authentication/microsoft-azure-blob-storage-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Azure
- Blobs
- Cloud Storage
- Microsoft
- Object Storage
- Storage
---
