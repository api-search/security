---
api_key_in: []
api_specs:
- filename: nanonets-external-integrations-api-openapi.yml
  format: yaml
  label: Nanonets External Integrations API
  slug: nanonets-external-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-external-integrations-api-openapi.yml
- filename: nanonets-file-assignment-api-openapi.yml
  format: yaml
  label: Nanonets File Assignment API
  slug: nanonets-file-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-assignment-api-openapi.yml
- filename: nanonets-file-delete-api-openapi.yml
  format: yaml
  label: Nanonets File Delete API
  slug: nanonets-file-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-delete-api-openapi.yml
- filename: nanonets-file-export-api-openapi.yml
  format: yaml
  label: Nanonets File Export API
  slug: nanonets-file-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-export-api-openapi.yml
- filename: nanonets-file-review-api-openapi.yml
  format: yaml
  label: Nanonets File Review API
  slug: nanonets-file-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-review-api-openapi.yml
- filename: nanonets-file-update-api-openapi.yml
  format: yaml
  label: Nanonets File Update API
  slug: nanonets-file-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-update-api-openapi.yml
- filename: nanonets-image-classification-predict-api-openapi.yml
  format: yaml
  label: Nanonets Image Classification Predict API
  slug: nanonets-image-classification-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-image-classification-predict-api-openapi.yml
- filename: nanonets-ocr-predict-api-openapi.yml
  format: yaml
  label: Nanonets OCR Predict API
  slug: nanonets-ocr-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-predict-api-openapi.yml
- filename: nanonets-ocr-retrieve-api-openapi.yml
  format: yaml
  label: Nanonets OCR Retrieve API
  slug: nanonets-ocr-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-retrieve-api-openapi.yml
- filename: nanonets-ocr-train-api-openapi.yml
  format: yaml
  label: Nanonets OCR Train API
  slug: nanonets-ocr-train-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-train-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nanonets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nanonets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nanonets
provider_slug: nanonets
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/nanonets-external-integrations-api-openapi.yml
  - openapi/nanonets-file-management-api-openapi.yml
  - openapi/nanonets-image-classification-api-openapi.yml
  - openapi/nanonets-ocr-api-openapi.yml
  type: http
slug: nanonets-authentication
source_filename: nanonets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nanonets-external-integrations-api-openapi.yml, openapi/nanonets-file-management-api-openapi.yml,\n  openapi/nanonets-image-classification-api-openapi.yml, openapi/nanonets-ocr-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nanonets-external-integrations-api-openapi.yml\n  - openapi/nanonets-file-management-api-openapi.yml\n  - openapi/nanonets-image-classification-api-openapi.yml\n  - openapi/nanonets-ocr-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/authentication/nanonets-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- OCR
- Document AI
- Intelligent Document Processing
- Data Extraction
- Workflow Automation
- Computer Vision
- No-Code
---
