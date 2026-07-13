---
api_key_in: []
api_specs:
- filename: llamaindex-llamacloud-api-openapi.yml
  format: yaml
  label: LlamaIndex LlamaCloud API
  slug: llamacloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-llamacloud-api-openapi.yml
- filename: llamaindex-llamaparse-api-openapi.yml
  format: yaml
  label: LlamaIndex LlamaParse API
  slug: llamaparse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-llamaparse-api-openapi.yml
- filename: llamaindex-llamaextract-api-openapi.yml
  format: yaml
  label: LlamaIndex LlamaExtract API
  slug: llamaextract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-llamaextract-api-openapi.yml
- filename: llamaindex-llamacloud-index-api-openapi.yml
  format: yaml
  label: LlamaIndex LlamaCloud Index API
  slug: llamacloud-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/openapi/llamaindex-llamacloud-index-api-openapi.yml
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
