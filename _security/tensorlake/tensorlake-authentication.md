---
api_key_in: []
api_specs:
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Document Parse API
  slug: tensorlake-document-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Structured Extraction API
  slug: tensorlake-structured-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Files API
  slug: tensorlake-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Datasets API
  slug: tensorlake-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Sandboxes API
  slug: tensorlake-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Tensorlake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tensorlake secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tensorlake
provider_slug: tensorlake
scheme_count: 1
schemes:
- description: 'Tensorlake API key created in the Tensorlake Cloud dashboard (cloud.tensorlake.ai) under a project. Keys are prefixed `tl_apiKey_` and are passed on every REST request as `Authorization: Bearer <token>`. A live unauthenticated request to https://api.tensorlake.ai returns HTTP 401, confirming Bearer enforcement.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.tensorlake.ai/platform/authentication
  - https://docs.tensorlake.ai/api-reference/introduction
  type: http
slug: tensorlake-authentication
source_filename: tensorlake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://docs.tensorlake.ai/platform/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Tensorlake API key created in the Tensorlake Cloud dashboard\n    (cloud.tensorlake.ai) under a project. Keys are prefixed `tl_apiKey_` and are\n    passed on every REST request as `Authorization: Bearer <token>`. A live\n    unauthenticated request to https://api.tensorlake.ai returns HTTP 401,\n    confirming Bearer enforcement.\n  sources:\n  - https://docs.tensorlake.ai/platform/authentication\n  - https://docs.tensorlake.ai/api-reference/introduction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/authentication/tensorlake-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Extraction
- Data Extraction
- Document Ingestion
- Document Parsing
- OCR
- Data Ingestion
- AI
- Unstructured Data
- Document AI
- RAG
---
