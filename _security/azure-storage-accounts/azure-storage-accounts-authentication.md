---
api_key_in: []
api_specs:
- filename: azure-storage-accounts-blobcontainers-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobContainers API
  slug: azure-storage-accounts-blobcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobcontainers-api-openapi.yml
- filename: azure-storage-accounts-blobservice-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobService API
  slug: azure-storage-accounts-blobservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobservice-api-openapi.yml
- filename: azure-storage-accounts-locationusage-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts LocationUsage API
  slug: azure-storage-accounts-locationusage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-locationusage-api-openapi.yml
- filename: azure-storage-accounts-managementpolicies-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts ManagementPolicies API
  slug: azure-storage-accounts-managementpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-managementpolicies-api-openapi.yml
- filename: azure-storage-accounts-operations-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Operations API
  slug: azure-storage-accounts-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-operations-api-openapi.yml
- filename: azure-storage-accounts-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateEndpointConnections API
  slug: azure-storage-accounts-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privateendpointconnections-api-openapi.yml
- filename: azure-storage-accounts-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateLinkResources API
  slug: azure-storage-accounts-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privatelinkresources-api-openapi.yml
- filename: azure-storage-accounts-skus-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Skus API
  slug: azure-storage-accounts-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-skus-api-openapi.yml
- filename: azure-storage-accounts-storageaccounts-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts StorageAccounts API
  slug: azure-storage-accounts-storageaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-storageaccounts-api-openapi.yml
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
