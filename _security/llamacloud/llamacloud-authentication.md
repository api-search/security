---
api_key_in: []
api_specs:
- filename: llamacloud-documents-api-openapi.yml
  format: yaml
  label: LlamaCloud Documents API
  slug: llamacloud-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-documents-api-openapi.yml
- filename: llamacloud-extraction-api-openapi.yml
  format: yaml
  label: LlamaCloud Extraction API
  slug: llamacloud-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-extraction-api-openapi.yml
- filename: llamacloud-parsing-api-openapi.yml
  format: yaml
  label: LlamaCloud Parsing API
  slug: llamacloud-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-parsing-api-openapi.yml
- filename: llamacloud-pipelines-api-openapi.yml
  format: yaml
  label: LlamaCloud Pipelines API
  slug: llamacloud-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-pipelines-api-openapi.yml
- filename: llamacloud-retrieval-api-openapi.yml
  format: yaml
  label: LlamaCloud Retrieval API
  slug: llamacloud-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-retrieval-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Llamacloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: LlamaCloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LlamaCloud
provider_slug: llamacloud
scheme_count: 1
schemes:
- description: LlamaCloud API key sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/llamacloud-openapi.yml
  type: http
slug: llamacloud-authentication
source_filename: llamacloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/llamacloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: LlamaCloud API key sent as a Bearer token.\n  sources:\n  - openapi/llamacloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/authentication/llamacloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Document Parsing
- Extraction
- Indexing
- Retrieval
- RAG
---
