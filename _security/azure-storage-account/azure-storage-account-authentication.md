---
api_key_in: []
api_specs:
- filename: blob.json
  format: json
  label: Azure Blob Storage API
  slug: azure-blob-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/data-plane/Microsoft.BlobStorage/stable/2021-12-02/blob.json
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure Queue Storage API
  slug: azure-queue-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure Table Storage API
  slug: azure-table-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure File Storage API
  slug: azure-file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Storage Account Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Storage Account secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Storage Account
provider_slug: azure-storage-account
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-storage-account-blob-openapi.yaml
  - openapi/azure-storage-account-management-openapi.yaml
  type: oauth2
slug: azure-storage-account-authentication
source_filename: azure-storage-account-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-storage-account-blob-openapi.yaml, openapi/azure-storage-account-management-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-storage-account-blob-openapi.yaml\n  - openapi/azure-storage-account-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/authentication/azure-storage-account-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
---
