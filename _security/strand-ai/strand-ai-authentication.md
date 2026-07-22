---
api_key_in: []
api_specs:
- filename: strand-ai-openapi-original.json
  format: json
  label: Strand Platform API
  slug: strand-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Strand Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strand AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Strand AI
provider_slug: strand-ai
scheme_count: 1
schemes:
- bearerFormat: sk-strand-XXXXXXXXXXXXXXXXXXXXXXXX
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/strand-ai-openapi-original.json
  type: http
slug: strand-ai-authentication
source_filename: strand-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/strand-ai-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: sk-strand-XXXXXXXXXXXXXXXXXXXXXXXX\n  sources:\n  - openapi/strand-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/authentication/strand-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Life Sciences
- Spatial Biology
- Bioinformatics
- Drug Discovery
- Foundation Models
- Digital Pathology
- Healthcare
---
