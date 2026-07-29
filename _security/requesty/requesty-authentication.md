---
api_key_in: []
api_specs:
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Chat Completions API
  slug: requesty-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Models API
  slug: requesty-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Usage & Analytics API
  slug: requesty-usage-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty API Keys API
  slug: requesty-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Requesty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Requesty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Requesty
provider_slug: requesty
scheme_count: 1
schemes:
- description: Requesty API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/requesty-openapi.yml
  type: http
slug: requesty-authentication
source_filename: requesty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/requesty-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Requesty API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/requesty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/authentication/requesty-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Routing
- Gateway
- Observability
---
