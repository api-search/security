---
api_key_in: []
api_specs:
- filename: azure-storage-account-blobcontainers-api-openapi.yml
  format: yaml
  label: Azure Storage Account BlobContainers API
  slug: azure-storage-account-blobcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-blobcontainers-api-openapi.yml
- filename: azure-storage-account-blobservice-api-openapi.yml
  format: yaml
  label: Azure Storage Account BlobService API
  slug: azure-storage-account-blobservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-blobservice-api-openapi.yml
- filename: azure-storage-account-locationusage-api-openapi.yml
  format: yaml
  label: Azure Storage Account LocationUsage API
  slug: azure-storage-account-locationusage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-locationusage-api-openapi.yml
- filename: azure-storage-account-managementpolicies-api-openapi.yml
  format: yaml
  label: Azure Storage Account ManagementPolicies API
  slug: azure-storage-account-managementpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-managementpolicies-api-openapi.yml
- filename: azure-storage-account-operations-api-openapi.yml
  format: yaml
  label: Azure Storage Account Operations API
  slug: azure-storage-account-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-operations-api-openapi.yml
- filename: azure-storage-account-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Azure Storage Account PrivateEndpointConnections API
  slug: azure-storage-account-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-privateendpointconnections-api-openapi.yml
- filename: azure-storage-account-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Storage Account PrivateLinkResources API
  slug: azure-storage-account-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-privatelinkresources-api-openapi.yml
- filename: azure-storage-account-skus-api-openapi.yml
  format: yaml
  label: Azure Storage Account Skus API
  slug: azure-storage-account-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-skus-api-openapi.yml
- filename: azure-storage-account-storageaccounts-api-openapi.yml
  format: yaml
  label: Azure Storage Account StorageAccounts API
  slug: azure-storage-account-storageaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-storageaccounts-api-openapi.yml
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
