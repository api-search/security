---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genomicintelligence-ai-health-api-openapi.yml
  format: yaml
  label: Genomic Intelligence Health API
  slug: genomicintelligence-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genomicintelligence-ai/openapi/genomicintelligence-ai-health-api-openapi.yml
- filename: genomicintelligence-ai-tasks-api-openapi.yml
  format: yaml
  label: Genomic Intelligence Tasks API
  slug: genomicintelligence-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genomicintelligence-ai/openapi/genomicintelligence-ai-tasks-api-openapi.yml
- filename: genomicintelligence-ai-workflows-api-openapi.yml
  format: yaml
  label: Genomic Intelligence Workflows API
  slug: genomicintelligence-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genomicintelligence-ai/openapi/genomicintelligence-ai-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Genomic Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genomic Intelligence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genomic Intelligence
provider_slug: genomicintelligence-ai
scheme_count: 1
schemes:
- bearerFormat: gi_…
  description: Partner API key. Issued out of band; see https://docs.genomicintelligence.ai/rest-api.md#2-get-a-key.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/genomicintelligence-ai-openapi.json
  type: http
slug: genomicintelligence-ai-authentication
source_filename: genomicintelligence-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/genomicintelligence-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: gi_…\n  description: Partner API key. Issued out of band; see https://docs.genomicintelligence.ai/rest-api.md#2-get-a-key.\n  sources:\n  - openapi/genomicintelligence-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/genomicintelligence-ai/authentication/genomicintelligence-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Genomics
- Artificial Intelligence
- Bioinformatics
- DNA
---
