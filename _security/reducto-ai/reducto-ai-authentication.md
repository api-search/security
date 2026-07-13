---
api_key_in: []
api_specs:
- filename: reducto-parse-api-openapi.yml
  format: yaml
  label: Reducto Parse API
  slug: reducto-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-parse-api-openapi.yml
- filename: reducto-extract-api-openapi.yml
  format: yaml
  label: Reducto Extract API
  slug: reducto-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-extract-api-openapi.yml
- filename: reducto-split-api-openapi.yml
  format: yaml
  label: Reducto Split API
  slug: reducto-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-split-api-openapi.yml
- filename: reducto-edit-api-openapi.yml
  format: yaml
  label: Reducto Edit API
  slug: reducto-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-edit-api-openapi.yml
- filename: reducto-pipeline-api-openapi.yml
  format: yaml
  label: Reducto Pipeline API
  slug: reducto-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-pipeline-api-openapi.yml
- filename: reducto-classify-api-openapi.yml
  format: yaml
  label: Reducto Classify API
  slug: reducto-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-classify-api-openapi.yml
- filename: reducto-jobs-api-openapi.yml
  format: yaml
  label: Reducto Jobs API
  slug: reducto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-jobs-api-openapi.yml
- filename: reducto-upload-api-openapi.yml
  format: yaml
  label: Reducto Upload API
  slug: reducto-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-upload-api-openapi.yml
- filename: reducto-webhooks-api-openapi.yml
  format: yaml
  label: Reducto Webhooks API
  slug: reducto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-webhooks-api-openapi.yml
- filename: reducto-platform-api-openapi.yml
  format: yaml
  label: Reducto Platform API
  slug: reducto-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reducto Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: reducto-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: reducto-ai
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
