---
api_key_in: []
api_specs:
- filename: blob.json
  format: json
  label: Azure Storage Blob Service API
  slug: azure-storage-blob-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/data-plane/Microsoft.BlobStorage/stable/2023-11-03/blob.json
- filename: storage.json
  format: json
  label: Azure Storage Management API
  slug: azure-storage-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/resource-manager/Microsoft.Storage/stable/2023-01-01/storage.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Storage Accounts Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Storage Accounts secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-storage-accounts-blob-openapi.yaml
  - openapi/azure-storage-accounts-management-openapi.yaml
  type: oauth2
slug: azure-storage-accounts-authentication
source_filename: azure-storage-accounts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-storage-accounts-blob-openapi.yaml, openapi/azure-storage-accounts-management-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-storage-accounts-blob-openapi.yaml\n  - openapi/azure-storage-accounts-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/authentication/azure-storage-accounts-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
---
