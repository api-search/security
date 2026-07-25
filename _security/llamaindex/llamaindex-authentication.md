---
api_key_in: []
api_specs:
- filename: llamaindex-data-sources-api-openapi.yml
  format: yaml
  label: llamaindex Data Sources API
  slug: llamaindex-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-data-sources-api-openapi.yml
- filename: llamaindex-extraction-agents-api-openapi.yml
  format: yaml
  label: llamaindex Extraction Agents API
  slug: llamaindex-extraction-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-extraction-agents-api-openapi.yml
- filename: llamaindex-extraction-jobs-api-openapi.yml
  format: yaml
  label: llamaindex Extraction Jobs API
  slug: llamaindex-extraction-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-extraction-jobs-api-openapi.yml
- filename: llamaindex-files-api-openapi.yml
  format: yaml
  label: llamaindex Files API
  slug: llamaindex-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-files-api-openapi.yml
- filename: llamaindex-index-data-sources-api-openapi.yml
  format: yaml
  label: llamaindex Index Data Sources API
  slug: llamaindex-index-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-index-data-sources-api-openapi.yml
- filename: llamaindex-index-files-api-openapi.yml
  format: yaml
  label: llamaindex Index Files API
  slug: llamaindex-index-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-index-files-api-openapi.yml
- filename: llamaindex-index-retrieval-api-openapi.yml
  format: yaml
  label: llamaindex Index Retrieval API
  slug: llamaindex-index-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-index-retrieval-api-openapi.yml
- filename: llamaindex-index-status-api-openapi.yml
  format: yaml
  label: llamaindex Index Status API
  slug: llamaindex-index-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-index-status-api-openapi.yml
- filename: llamaindex-indexes-api-openapi.yml
  format: yaml
  label: llamaindex Indexes API
  slug: llamaindex-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-indexes-api-openapi.yml
- filename: llamaindex-jobs-api-openapi.yml
  format: yaml
  label: llamaindex Jobs API
  slug: llamaindex-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-jobs-api-openapi.yml
- filename: llamaindex-parsing-api-openapi.yml
  format: yaml
  label: llamaindex Parsing API
  slug: llamaindex-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-parsing-api-openapi.yml
- filename: llamaindex-pipeline-data-sinks-api-openapi.yml
  format: yaml
  label: llamaindex Pipeline Data Sinks API
  slug: llamaindex-pipeline-data-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-pipeline-data-sinks-api-openapi.yml
- filename: llamaindex-pipeline-data-sources-api-openapi.yml
  format: yaml
  label: llamaindex Pipeline Data Sources API
  slug: llamaindex-pipeline-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-pipeline-data-sources-api-openapi.yml
- filename: llamaindex-pipeline-files-api-openapi.yml
  format: yaml
  label: llamaindex Pipeline Files API
  slug: llamaindex-pipeline-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-pipeline-files-api-openapi.yml
- filename: llamaindex-pipeline-jobs-api-openapi.yml
  format: yaml
  label: llamaindex Pipeline Jobs API
  slug: llamaindex-pipeline-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-pipeline-jobs-api-openapi.yml
- filename: llamaindex-pipelines-api-openapi.yml
  format: yaml
  label: llamaindex Pipelines API
  slug: llamaindex-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-pipelines-api-openapi.yml
- filename: llamaindex-projects-api-openapi.yml
  format: yaml
  label: llamaindex Projects API
  slug: llamaindex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-projects-api-openapi.yml
- filename: llamaindex-retrieval-api-openapi.yml
  format: yaml
  label: llamaindex Retrieval API
  slug: llamaindex-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-retrieval-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Llamaindex Authentication
name_suffix: Authentication
oauth_flows: []
overview: llamaindex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: llamaindex
provider_slug: llamaindex
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: LlamaCloud API key obtained from the LlamaCloud dashboard. Include as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/llamaindex-llamacloud-api-openapi.yml
  - openapi/llamaindex-llamacloud-index-api-openapi.yml
  - openapi/llamaindex-llamaextract-api-openapi.yml
  - openapi/llamaindex-llamaparse-api-openapi.yml
  type: http
slug: llamaindex-authentication
source_filename: llamaindex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/llamaindex-llamacloud-api-openapi.yml, openapi/llamaindex-llamacloud-index-api-openapi.yml,\n  openapi/llamaindex-llamaextract-api-openapi.yml, openapi/llamaindex-llamaparse-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: LlamaCloud API key obtained from the LlamaCloud dashboard. Include as a Bearer\n    token in the Authorization header.\n  sources:\n  - openapi/llamaindex-llamacloud-api-openapi.yml\n  - openapi/llamaindex-llamacloud-index-api-openapi.yml\n  - openapi/llamaindex-llamaextract-api-openapi.yml\n  - openapi/llamaindex-llamaparse-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/authentication/llamaindex-authentication.yml
summary_line: http · 1 scheme
tags: []
---
