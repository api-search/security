---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: docupanda-analysis-api-openapi.yml
  format: yaml
  label: DocuPipe Analysis API
  slug: docupanda-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-analysis-api-openapi.yml
- filename: docupanda-account-api-openapi.yml
  format: yaml
  label: DocuPipe Account API
  slug: docupanda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-account-api-openapi.yml
- filename: docupanda-account-api-openapi.yml
  format: yaml
  label: DocuPipe Account API
  slug: docupanda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-account-api-openapi.yml
- filename: docupanda-analysis-api-openapi.yml
  format: yaml
  label: DocuPipe Analysis API
  slug: docupanda-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-analysis-api-openapi.yml
- filename: docupanda-classification-api-openapi.yml
  format: yaml
  label: DocuPipe Classification API
  slug: docupanda-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-classification-api-openapi.yml
- filename: docupanda-document-api-openapi.yml
  format: yaml
  label: DocuPipe Document API
  slug: docupanda-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-document-api-openapi.yml
- filename: docupanda-job-api-openapi.yml
  format: yaml
  label: DocuPipe Job API
  slug: docupanda-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-job-api-openapi.yml
- filename: docupanda-review-api-openapi.yml
  format: yaml
  label: DocuPipe Review API
  slug: docupanda-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-review-api-openapi.yml
- filename: docupanda-schema-api-openapi.yml
  format: yaml
  label: DocuPipe Schema API
  slug: docupanda-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-schema-api-openapi.yml
- filename: docupanda-standardization-api-openapi.yml
  format: yaml
  label: DocuPipe Standardization API
  slug: docupanda-standardization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-standardization-api-openapi.yml
- filename: docupanda-transformation-api-openapi.yml
  format: yaml
  label: DocuPipe Transformation API
  slug: docupanda-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-transformation-api-openapi.yml
- filename: docupanda-webhook-api-openapi.yml
  format: yaml
  label: DocuPipe Webhook API
  slug: docupanda-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-webhook-api-openapi.yml
- filename: docupanda-workflow-api-openapi.yml
  format: yaml
  label: DocuPipe Workflow API
  slug: docupanda-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-workflow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Docupanda Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocuPipe secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DocuPipe
provider_slug: docupanda
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/docupanda-docupipe-openapi.yml
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/docupanda-docupipe-openapi.yml
  type: http
slug: docupanda-authentication
source_filename: docupanda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/docupanda-docupipe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/docupanda-docupipe-openapi.yml\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/docupanda-docupipe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/authentication/docupanda-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Document Extraction
- Document Intelligence
- Intelligent Document Processing
- OCR
- Document AI
---
