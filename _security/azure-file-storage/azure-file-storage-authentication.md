---
api_key_in:
- header
api_specs:
- filename: azure-file-storage-openapi.yml
  format: yaml
  label: Azure Files FileREST API
  slug: filerest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-file-storage/refs/heads/main/openapi/azure-file-storage-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure File Storage Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azure Files secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azure Files
provider_slug: azure-file-storage
scheme_count: 2
schemes:
- description: 'Shared Key authorization header in the form `SharedKey {account}:{signature}`,

    where signature is an HMAC-SHA256 of the canonicalized request.

    See https://learn.microsoft.com/en-us/rest/api/storageservices/authorize-with-shared-key'
  in: header
  name: sharedKey
  parameter: Authorization
  sources:
  - openapi/azure-file-storage-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-file-storage-openapi.yml
  type: oauth2
slug: azure-file-storage-authentication
source_filename: azure-file-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-file-storage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Shared Key authorization header in the form `SharedKey {account}:{signature}`,\n    where signature is an HMAC-SHA256 of the canonicalized request.\n    See https://learn.microsoft.com/en-us/rest/api/storageservices/authorize-with-shared-key\n  sources:\n  - openapi/azure-file-storage-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n  sources:\n  - openapi/azure-file-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-file-storage/refs/heads/main/authentication/azure-file-storage-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Storage
- File Storage
- File Shares
- SMB
- NFS
- Cloud
- Azure
---
