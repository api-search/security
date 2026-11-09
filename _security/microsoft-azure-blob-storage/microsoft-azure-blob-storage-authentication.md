---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Append Blobs API
  slug: microsoft-azure-blob-storage-append-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
- filename: blob.json
  format: json
  label: Azure Blob Storage Azure Blob Storage REST API
  slug: microsoft-azure-blob-storage-azure-blob-storage-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/data-plane/BlobStorage/stable/2026-10-06/blob.json
- filename: microsoft-azure-blob-storage-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Blobs API
  slug: microsoft-azure-blob-storage-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Block Blobs API
  slug: microsoft-azure-blob-storage-block-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-containers-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Containers API
  slug: microsoft-azure-blob-storage-containers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
- filename: microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Page Blobs API
  slug: microsoft-azure-blob-storage-page-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-appendblob-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Appendblob API
  slug: microsoft-azure-blob-storage-appendblob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-appendblob-api-openapi.yml
- filename: microsoft-azure-blob-storage-blob-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Blob API
  slug: microsoft-azure-blob-storage-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-blob-api-openapi.yml
- filename: microsoft-azure-blob-storage-blockblob-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Blockblob API
  slug: microsoft-azure-blob-storage-blockblob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-blockblob-api-openapi.yml
- filename: microsoft-azure-blob-storage-container-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Container API
  slug: microsoft-azure-blob-storage-container-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-container-api-openapi.yml
- filename: microsoft-azure-blob-storage-pageblob-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Pageblob API
  slug: microsoft-azure-blob-storage-pageblob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-pageblob-api-openapi.yml
- filename: microsoft-azure-blob-storage-service-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Service API
  slug: microsoft-azure-blob-storage-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-blob-storage/openapi/microsoft-azure-blob-storage-service-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
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
  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: http
- description: Shared access signature (SAS) token granting delegated access to blob resources.
  in: query
  name: sharedAccessSignature
  parameter: sig
  sources:
  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  type: apiKey
slug: microsoft-azure-blob-storage-authentication
source_filename: microsoft-azure-blob-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml, openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml,\n  openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml, openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml,\n  openapi/microsoft-azure-blob-storage-containers-api-openapi.yml, openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Azure Storage shared key authorization using the storage account access key.\n  sources:\n  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n\
  \  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Microsoft Entra ID OAuth 2.0 bearer token for accessing blob resources.\n  sources:\n  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n- name: sharedAccessSignature\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared access signature (SAS) token granting delegated access to blob resources.\n  sources:\n  - openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml\n\
  \  - openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-containers-api-openapi.yml\n  - openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml\n"
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
