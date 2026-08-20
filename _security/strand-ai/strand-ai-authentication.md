---
api_key_in: []
api_specs:
- filename: strand-ai-jobs-api-openapi.yml
  format: yaml
  label: Strand AI Jobs API
  slug: strand-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-jobs-api-openapi.yml
- filename: strand-ai-predict-api-openapi.yml
  format: yaml
  label: Strand AI Predict API
  slug: strand-ai-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-predict-api-openapi.yml
- filename: strand-ai-samples-api-openapi.yml
  format: yaml
  label: Strand AI Samples API
  slug: strand-ai-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-samples-api-openapi.yml
- filename: strand-ai-uploads-api-openapi.yml
  format: yaml
  label: Strand AI Uploads API
  slug: strand-ai-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-uploads-api-openapi.yml
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
- Machine-Learning
- Life Sciences
- Spatial Biology
- Bioinformatics
- Drug Discovery
- Foundation Models
- Digital Pathology
- Healthcare
---
