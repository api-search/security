---
api_key_in:
- header
api_specs:
- filename: unstructured-channels-api-openapi.yml
  format: yaml
  label: Unstructured channels API
  slug: unstructured-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-channels-api-openapi.yml
- filename: unstructured-destinations-api-openapi.yml
  format: yaml
  label: Unstructured destinations API
  slug: unstructured-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-destinations-api-openapi.yml
- filename: unstructured-general-api-openapi.yml
  format: yaml
  label: Unstructured general API
  slug: unstructured-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-general-api-openapi.yml
- filename: unstructured-jobs-api-openapi.yml
  format: yaml
  label: Unstructured jobs API
  slug: unstructured-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-jobs-api-openapi.yml
- filename: unstructured-notifications-api-openapi.yml
  format: yaml
  label: Unstructured notifications API
  slug: unstructured-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-notifications-api-openapi.yml
- filename: unstructured-sources-api-openapi.yml
  format: yaml
  label: Unstructured sources API
  slug: unstructured-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-sources-api-openapi.yml
- filename: unstructured-templates-api-openapi.yml
  format: yaml
  label: Unstructured templates API
  slug: unstructured-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-templates-api-openapi.yml
- filename: unstructured-workflow-channels-api-openapi.yml
  format: yaml
  label: Unstructured workflow-channels API
  slug: unstructured-workflow-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-workflow-channels-api-openapi.yml
- filename: unstructured-workflows-api-openapi.yml
  format: yaml
  label: Unstructured workflows API
  slug: unstructured-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unstructured Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unstructured secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unstructured
provider_slug: unstructured
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: unstructured-api-key
  sources:
  - openapi/unstructured-partition-endpoint-openapi.yml
  type: apiKey
slug: unstructured-authentication
source_filename: unstructured-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unstructured-partition-endpoint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: unstructured-api-key\n  sources:\n  - openapi/unstructured-partition-endpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/authentication/unstructured-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Processing
- ETL
- RAG
- LLM
- PDF
- OCR
- Data Ingestion
- Chunking
- Embeddings
- Artificial Intelligence
---
