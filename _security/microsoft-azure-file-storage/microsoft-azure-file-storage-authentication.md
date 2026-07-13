---
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-file-storage-openapi.yml
  format: yaml
  label: Azure File Storage REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-file-storage/refs/heads/main/openapi/microsoft-azure-file-storage-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure File Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure File Storage secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure File Storage
provider_slug: microsoft-azure-file-storage
scheme_count: 2
schemes:
- description: Shared Key authentication
  in: header
  name: sharedKey
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-file-storage-openapi.yml
  type: apiKey
- description: Shared Access Signature token
  in: query
  name: sasToken
  parameter: sig
  sources:
  - openapi/microsoft-azure-file-storage-openapi.yml
  type: apiKey
slug: microsoft-azure-file-storage-authentication
source_filename: microsoft-azure-file-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-file-storage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Shared Key authentication\n  sources:\n  - openapi/microsoft-azure-file-storage-openapi.yml\n- name: sasToken\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared Access Signature token\n  sources:\n  - openapi/microsoft-azure-file-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-file-storage/refs/heads/main/authentication/microsoft-azure-file-storage-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cloud Storage
- File Shares
- File Storage
- NFS
- SMB
---
