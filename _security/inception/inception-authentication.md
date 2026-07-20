---
api_key_in: []
api_specs:
- filename: inception-openapi-original.json
  format: json
  label: Inception API
  slug: inception-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception/refs/heads/main/openapi/inception-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Inception Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inception secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inception
provider_slug: inception
scheme_count: 1
schemes:
- description: 'API key provided as a Bearer token: `Authorization: Bearer <api_key>`. Get an API key at https://platform.inceptionlabs.ai.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/inception-openapi-original.json
  type: http
slug: inception-authentication
source_filename: inception-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/inception-openapi-original.json\ndocs: https://docs.inceptionlabs.ai/get-started/authentication\nenv_var: INCEPTION_API_KEY\nkey_management: https://platform.inceptionlabs.ai/dashboard/api-keys\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key provided as a Bearer token: `Authorization: Bearer <api_key>`. Get an\n    API key at https://platform.inceptionlabs.ai.'\n  sources:\n  - openapi/inception-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inception/refs/heads/main/authentication/inception-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- LLM
- Artificial Intelligence
- Diffusion Models
- Code Completion
- Machine Learning
- Developer Tools
---
