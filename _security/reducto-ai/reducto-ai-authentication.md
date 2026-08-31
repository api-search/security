---
api_key_in: []
api_specs:
- filename: reducto-ai-classify-api-openapi.yml
  format: yaml
  label: reducto-ai Classify API
  slug: reducto-ai-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-classify-api-openapi.yml
- filename: reducto-ai-edit-api-openapi.yml
  format: yaml
  label: reducto-ai Edit API
  slug: reducto-ai-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-edit-api-openapi.yml
- filename: reducto-ai-extract-api-openapi.yml
  format: yaml
  label: reducto-ai Extract API
  slug: reducto-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-extract-api-openapi.yml
- filename: reducto-ai-jobs-api-openapi.yml
  format: yaml
  label: reducto-ai Jobs API
  slug: reducto-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-jobs-api-openapi.yml
- filename: reducto-ai-parse-api-openapi.yml
  format: yaml
  label: reducto-ai Parse API
  slug: reducto-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-parse-api-openapi.yml
- filename: reducto-ai-pipeline-api-openapi.yml
  format: yaml
  label: reducto-ai Pipeline API
  slug: reducto-ai-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-pipeline-api-openapi.yml
- filename: reducto-ai-platform-api-openapi.yml
  format: yaml
  label: reducto-ai Platform API
  slug: reducto-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-platform-api-openapi.yml
- filename: reducto-ai-split-api-openapi.yml
  format: yaml
  label: reducto-ai Split API
  slug: reducto-ai-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-split-api-openapi.yml
- filename: reducto-ai-upload-api-openapi.yml
  format: yaml
  label: reducto-ai Upload API
  slug: reducto-ai-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-upload-api-openapi.yml
- filename: reducto-ai-webhooks-api-openapi.yml
  format: yaml
  label: reducto-ai Webhooks API
  slug: reducto-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reducto Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reducto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reducto
provider_slug: reducto-ai
scheme_count: 1
schemes:
- name: SkippableHTTPBearer
  scheme: bearer
  sources:
  - openapi/reducto-classify-api-openapi.yml
  - openapi/reducto-edit-api-openapi.yml
  - openapi/reducto-extract-api-openapi.yml
  - openapi/reducto-jobs-api-openapi.yml
  - openapi/reducto-parse-api-openapi.yml
  - openapi/reducto-pipeline-api-openapi.yml
  - openapi/reducto-platform-api-openapi.yml
  - openapi/reducto-split-api-openapi.yml
  - openapi/reducto-upload-api-openapi.yml
  - openapi/reducto-webhooks-api-openapi.yml
  type: http
slug: reducto-ai-authentication
source_filename: reducto-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reducto-classify-api-openapi.yml, openapi/reducto-edit-api-openapi.yml, openapi/reducto-extract-api-openapi.yml,\n  openapi/reducto-jobs-api-openapi.yml, openapi/reducto-parse-api-openapi.yml, openapi/reducto-pipeline-api-openapi.yml,\n  openapi/reducto-platform-api-openapi.yml, openapi/reducto-split-api-openapi.yml, openapi/reducto-upload-api-openapi.yml,\n  openapi/reducto-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: SkippableHTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/reducto-classify-api-openapi.yml\n  - openapi/reducto-edit-api-openapi.yml\n  - openapi/reducto-extract-api-openapi.yml\n  - openapi/reducto-jobs-api-openapi.yml\n  - openapi/reducto-parse-api-openapi.yml\n  - openapi/reducto-pipeline-api-openapi.yml\n  - openapi/reducto-platform-api-openapi.yml\n  - openapi/reducto-split-api-openapi.yml\n  - openapi/reducto-upload-api-openapi.yml\n  - openapi/reducto-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/authentication/reducto-ai-authentication.yml
summary_line: http · 1 scheme
tags: []
---
