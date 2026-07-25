---
api_key_in: []
api_specs:
- filename: extend-ai-batch-api-openapi.yml
  format: yaml
  label: Extend Batch API
  slug: extend-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-batch-api-openapi.yml
- filename: extend-ai-classify-api-openapi.yml
  format: yaml
  label: Extend Classify API
  slug: extend-ai-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-classify-api-openapi.yml
- filename: extend-ai-evaluations-api-openapi.yml
  format: yaml
  label: Extend Evaluations API
  slug: extend-ai-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-evaluations-api-openapi.yml
- filename: extend-ai-extract-api-openapi.yml
  format: yaml
  label: Extend Extract API
  slug: extend-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-extract-api-openapi.yml
- filename: extend-ai-files-api-openapi.yml
  format: yaml
  label: Extend Files API
  slug: extend-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-files-api-openapi.yml
- filename: extend-ai-parse-api-openapi.yml
  format: yaml
  label: Extend Parse API
  slug: extend-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-parse-api-openapi.yml
- filename: extend-ai-split-api-openapi.yml
  format: yaml
  label: Extend Split API
  slug: extend-ai-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-split-api-openapi.yml
- filename: extend-ai-workflow-runs-api-openapi.yml
  format: yaml
  label: Extend Workflow Runs API
  slug: extend-ai-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-workflow-runs-api-openapi.yml
- filename: extend-ai-workflows-api-openapi.yml
  format: yaml
  label: Extend Workflows API
  slug: extend-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Extend Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Extend
provider_slug: extend-ai
scheme_count: 1
schemes:
- description: Provide your Extend API token as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/extend-ai-openapi.yml
  type: http
slug: extend-ai-authentication
source_filename: extend-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/extend-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Provide your Extend API token as a Bearer token in the Authorization header.\n  sources:\n  - openapi/extend-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/authentication/extend-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Processing
- Document AI
- Intelligent Document Processing
- OCR
- Extraction
- Classification
---
