---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eshmere-ai-drafting-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Drafting API
  slug: eshmere-ai-drafting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-drafting-api-openapi.yml
- filename: eshmere-ai-pipeline-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Pipeline API
  slug: eshmere-ai-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-pipeline-api-openapi.yml
- filename: eshmere-ai-read-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Read API
  slug: eshmere-ai-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-read-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eshmere Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eshmere Ltd secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eshmere Ltd
provider_slug: eshmere-ai
scheme_count: 1
schemes:
- description: A Winquill API key, starting tk_live_, or the test key tk_test_sample.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/eshmere-ai-openapi.json
  type: http
slug: eshmere-ai-authentication
source_filename: eshmere-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eshmere-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: A Winquill API key, starting tk_live_, or the test key tk_test_sample.\n  sources:\n  - openapi/eshmere-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eshmere-ai/authentication/eshmere-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Public Procurement
- Real Estate
- Automation
- Software-as-a-Service
---
