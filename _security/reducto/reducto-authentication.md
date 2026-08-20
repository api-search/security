---
api_key_in: []
api_specs:
- filename: reducto-cancel-api-openapi.yml
  format: yaml
  label: Reducto Cancel API
  slug: reducto-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-cancel-api-openapi.yml
- filename: reducto-classify-api-openapi.yml
  format: yaml
  label: Reducto Classify API
  slug: reducto-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-classify-api-openapi.yml
- filename: reducto-configure-webhook-api-openapi.yml
  format: yaml
  label: Reducto Configure Webhook API
  slug: reducto-configure-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-configure-webhook-api-openapi.yml
- filename: reducto-edit-api-openapi.yml
  format: yaml
  label: Reducto Edit API
  slug: reducto-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-api-openapi.yml
- filename: reducto-edit-async-api-openapi.yml
  format: yaml
  label: Reducto Edit Async API
  slug: reducto-edit-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-async-api-openapi.yml
- filename: reducto-extract-api-openapi.yml
  format: yaml
  label: Reducto Extract API
  slug: reducto-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-api-openapi.yml
- filename: reducto-extract-async-api-openapi.yml
  format: yaml
  label: Reducto Extract Async API
  slug: reducto-extract-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-async-api-openapi.yml
- filename: reducto-job-api-openapi.yml
  format: yaml
  label: Reducto Job API
  slug: reducto-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-job-api-openapi.yml
- filename: reducto-jobs-api-openapi.yml
  format: yaml
  label: Reducto Jobs API
  slug: reducto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-jobs-api-openapi.yml
- filename: reducto-parse-api-openapi.yml
  format: yaml
  label: Reducto Parse API
  slug: reducto-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-api-openapi.yml
- filename: reducto-parse-async-api-openapi.yml
  format: yaml
  label: Reducto Parse Async API
  slug: reducto-parse-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-async-api-openapi.yml
- filename: reducto-pipeline-api-openapi.yml
  format: yaml
  label: Reducto Pipeline API
  slug: reducto-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-api-openapi.yml
- filename: reducto-pipeline-async-api-openapi.yml
  format: yaml
  label: Reducto Pipeline Async API
  slug: reducto-pipeline-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-async-api-openapi.yml
- filename: reducto-split-api-openapi.yml
  format: yaml
  label: Reducto Split API
  slug: reducto-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-api-openapi.yml
- filename: reducto-split-async-api-openapi.yml
  format: yaml
  label: Reducto Split Async API
  slug: reducto-split-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-async-api-openapi.yml
- filename: reducto-upload-api-openapi.yml
  format: yaml
  label: Reducto Upload API
  slug: reducto-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-upload-api-openapi.yml
- filename: reducto-version-api-openapi.yml
  format: yaml
  label: Reducto Version API
  slug: reducto-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reducto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reducto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reducto
provider_slug: reducto
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/reducto-document-api-openapi.yml
  type: http
slug: reducto-authentication
source_filename: reducto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reducto-document-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/reducto-document-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/authentication/reducto-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Parsing
- PDF
- OCR
- Data Extraction
- Artificial Intelligence
- Machine-Learning
- Document Intelligence
- Structured Data
---
