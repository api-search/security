---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Modular Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modular secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Modular
provider_slug: modular
scheme_count: 2
schemes:
- context: hosted
  format: Bearer <API token>
  header: Authorization
  location: header
  name: bearerToken
  notes: The hosted Modular inference API (base https://api.modular.com/v1) requires a Bearer API token issued from the Modular Console; api.modular.com/v1/models returns HTTP 401 without one. API tokens are provisioned and billed per Organization.
  scheme: bearer
  type: http
- context: self-hosted
  location: header
  name: localNoAuth
  notes: Self-hosted `max serve` accepts the OpenAI api_key parameter for client compatibility but does not validate it (docs use api_key='EMPTY').
  scheme: bearer
  type: http
slug: modular-authentication
source_filename: modular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.modular.com/max/rest-api/\ndocs: https://docs.modular.com/max/inference/text-to-text/\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: Bearer <API token>\n    context: hosted\n    notes: >-\n      The hosted Modular inference API (base https://api.modular.com/v1) requires a\n      Bearer API token issued from the Modular Console; api.modular.com/v1/models\n      returns HTTP 401 without one. API tokens are provisioned and billed per Organization.\n  - name: localNoAuth\n    type: http\n    scheme: bearer\n    location: header\n    context: self-hosted\n    notes: >-\n      Self-hosted `max serve` accepts the OpenAI api_key parameter for client\n      compatibility but does not validate it (docs use api_key='EMPTY').\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modular/refs/heads/main/authentication/modular-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- GPU
- Developer Tools
- Infrastructure
---
