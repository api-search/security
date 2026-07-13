---
api_key_in: []
api_specs:
- filename: targon-openapi.yml
  format: yaml
  label: Targon Chat Completions API
  slug: targon-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Completions API
  slug: targon-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Models API
  slug: targon-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Images API
  slug: targon-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Search API
  slug: targon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Targon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Targon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Targon
provider_slug: targon
scheme_count: 1
schemes:
- description: 'Targon API key passed as a Bearer token in the Authorization header: `Authorization: Bearer $TARGON_API_KEY`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/targon-openapi.yml
  type: http
slug: targon-authentication
source_filename: targon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/targon-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Targon API key passed as a Bearer token in the Authorization header: `Authorization:\n    Bearer $TARGON_API_KEY`.'\n  sources:\n  - openapi/targon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/authentication/targon-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Decentralized
- Bittensor
---
