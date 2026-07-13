---
api_key_in: []
api_specs:
- filename: replicate-openapi.yml
  format: yaml
  label: Replicate
  slug: replicate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Replicate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replicate
provider_slug: replicate
scheme_count: 1
schemes:
- bearerFormat: 'All API requests must include a valid API token in the `Authorization` request header. The token must be prefixed by "Bearer", followed by a space and the token value.

    Example: `Authorization: Bearer r8_Hw***********************************`

    Find your tokens at https://replicate.com/account/api-tokens

    '
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/replicate-openapi.yml
  type: http
slug: replicate-authentication
source_filename: replicate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/replicate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: |\n    All API requests must include a valid API token in the `Authorization` request header. The token must be prefixed by \"Bearer\", followed by a space and the token value.\n    Example: `Authorization: Bearer r8_Hw***********************************`\n    Find your tokens at https://replicate.com/account/api-tokens\n  sources:\n  - openapi/replicate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/authentication/replicate-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- Image Generation
- Language Models
- Model Deployment
---
