---
api_key_in: []
api_specs:
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Processors API
  slug: processors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Processor Runs API
  slug: processor-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Workflows API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Workflow Runs API
  slug: workflow-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Evaluations API
  slug: evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
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
