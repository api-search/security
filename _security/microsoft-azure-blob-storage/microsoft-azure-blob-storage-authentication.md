---
api_key_in:
- header
- query
api_specs:
- filename: blob.json
  format: json
  label: Azure Blob Storage REST API
  slug: azure-blob-storage-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/data-plane/Microsoft.BlobStorage/stable/2021-12-02/blob.json
- filename: storage.json
  format: json
  label: Azure Storage Resource Provider REST API
  slug: azure-storage-resource-provider-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/resource-manager/Microsoft.Storage/stable/2023-05-01/storage.json
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
