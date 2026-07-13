---
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-data-lake-openapi.yml
  format: yaml
  label: Azure Data Lake Storage REST API
  slug: azure-data-lake-storage-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-data-lake/refs/heads/main/openapi/microsoft-azure-data-lake-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Data Lake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Data Lake Storage secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure Data Lake Storage
provider_slug: microsoft-azure-data-lake
scheme_count: 2
schemes:
- description: Shared Key authentication
  in: header
  name: sharedKey
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-data-lake-openapi.yml
  type: apiKey
- description: Shared Access Signature token
  in: query
  name: sasToken
  parameter: sig
  sources:
  - openapi/microsoft-azure-data-lake-openapi.yml
  type: apiKey
slug: microsoft-azure-data-lake-authentication
source_filename: microsoft-azure-data-lake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-data-lake-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Shared Key authentication\n  sources:\n  - openapi/microsoft-azure-data-lake-openapi.yml\n- name: sasToken\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared Access Signature token\n  sources:\n  - openapi/microsoft-azure-data-lake-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-data-lake/refs/heads/main/authentication/microsoft-azure-data-lake-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Big Data
- Data Lake
- Hierarchical Storage
---
