---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aleph Alpha2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aleph Alpha2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aleph Alpha2
provider_slug: aleph-alpha2
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'API requests are authenticated with a bearer token supplied in the Authorization header (Authorization: Bearer <token>). Tokens are created in the Aleph Alpha account portal at https://app.aleph-alpha.com and passed to the official client via the `token` constructor parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.aleph-alpha.com/products/apis/pharia-inference/
  - https://github.com/Aleph-Alpha/aleph-alpha-client
  token_issuer: https://app.aleph-alpha.com
  type: http
slug: aleph-alpha2-authentication
source_filename: aleph-alpha2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.aleph-alpha.com/products/apis/pharia-inference/\ndocs: https://docs.aleph-alpha.com/products/apis/pharia-inference/\nnote: >-\n  Aleph Alpha does not publish a public OpenAPI document — the PhariaInference\n  API host (https://api.aleph-alpha.com) returns HTTP 401 on all unauthenticated\n  requests, including /.well-known/* and /openapi.json. This profile is derived\n  from the public documentation and the official aleph-alpha-client library.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: >-\n    API requests are authenticated with a bearer token supplied in the\n    Authorization header (Authorization: Bearer <token>). Tokens are created in\n    the Aleph Alpha account portal at https://app.aleph-alpha.com and passed to\n    the official client via the `token` constructor parameter.\n  token_issuer:\
  \ https://app.aleph-alpha.com\n  sources:\n  - https://docs.aleph-alpha.com/products/apis/pharia-inference/\n  - https://github.com/Aleph-Alpha/aleph-alpha-client\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha2/refs/heads/main/authentication/aleph-alpha2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Machine Learning
- Generative AI
- Sovereign AI
- Inference API
- Embeddings
- Europe
- Germany
- Enterprise AI
---
