---
api_key_in: []
api_specs:
- filename: friendliai-openapi-original.yml
  format: yaml
  label: Friendli Suite API
  slug: friendli-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendliai/refs/heads/main/openapi/friendliai-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Friendliai Authentication
name_suffix: Authentication
oauth_flows: []
overview: FriendliAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FriendliAI
provider_slug: friendliai
scheme_count: 1
schemes:
- description: 'When using Friendli Suite API for inference requests, you need to provide a **Friendli Token** for authentication and authorization purposes.


    For more detailed information, please refer [here](https://friendli.ai/docs/openapi/introduction#authentication).'
  name: token
  scheme: bearer
  sources:
  - openapi/friendliai-openapi-original.yml
  type: http
slug: friendliai-authentication
source_filename: friendliai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/friendliai-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: |-\n    When using Friendli Suite API for inference requests, you need to provide a **Friendli Token** for authentication and authorization purposes.\n\n    For more detailed information, please refer [here](https://friendli.ai/docs/openapi/introduction#authentication).\n  sources:\n  - openapi/friendliai-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendliai/refs/heads/main/authentication/friendliai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Infrastructure
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Generative AI
- GPU
- OpenAI Compatible
---
