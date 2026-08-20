---
api_key_in: []
api_specs:
- filename: biolevate-agent-api-openapi.yml
  format: yaml
  label: Biolevate Agent API
  slug: biolevate-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-agent-api-openapi.yml
- filename: biolevate-collections-api-openapi.yml
  format: yaml
  label: Biolevate Collections API
  slug: biolevate-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-collections-api-openapi.yml
- filename: biolevate-extraction-api-openapi.yml
  format: yaml
  label: Biolevate Extraction API
  slug: biolevate-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-extraction-api-openapi.yml
- filename: biolevate-files-api-openapi.yml
  format: yaml
  label: Biolevate Files API
  slug: biolevate-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-files-api-openapi.yml
- filename: biolevate-find-similar-files-api-openapi.yml
  format: yaml
  label: Biolevate Find similar files API
  slug: biolevate-find-similar-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-find-similar-files-api-openapi.yml
- filename: biolevate-multi-dimensional-extraction-api-openapi.yml
  format: yaml
  label: Biolevate Multi-Dimensional Extraction API
  slug: biolevate-multi-dimensional-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-multi-dimensional-extraction-api-openapi.yml
- filename: biolevate-provider-items-api-openapi.yml
  format: yaml
  label: Biolevate Provider Items API
  slug: biolevate-provider-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-provider-items-api-openapi.yml
- filename: biolevate-providers-api-openapi.yml
  format: yaml
  label: Biolevate Providers API
  slug: biolevate-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-providers-api-openapi.yml
- filename: biolevate-question-answering-api-openapi.yml
  format: yaml
  label: Biolevate Question Answering API
  slug: biolevate-question-answering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-question-answering-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Biolevate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biolevate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Biolevate
provider_slug: biolevate
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: TOKEN
  scheme: bearer
  sources:
  - openapi/biolevate-api-original.json
  type: http
slug: biolevate-authentication
source_filename: biolevate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/biolevate-api-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: TOKEN\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/biolevate-api-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/authentication/biolevate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Life Sciences
- Regulatory Affairs
- Document Intelligence
- Knowledge-Management
- Pharmaceuticals
- Machine-Learning
---
