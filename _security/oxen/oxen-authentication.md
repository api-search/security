---
api_key_in: []
api_specs:
- filename: oxen-hub-api-openapi-original.json
  format: json
  label: Oxen Hub AI & Fine-Tuning API
  slug: oxen-hub-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-hub-api-openapi-original.json
- filename: oxen-server-openapi-original.json
  format: json
  label: Oxen Data Version Control Server API
  slug: oxen-data-version-control-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-server-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Oxen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oxen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oxen
provider_slug: oxen
scheme_count: 1
schemes:
- description: 'Bearer API key. Header `Authorization: Bearer <OXEN_API_KEY>`. Same key across inference, fine-tuning, and version-control endpoints.'
  name: authorization
  scheme: bearer
  sources:
  - openapi/oxen-hub-api-openapi-original.json
  - openapi/oxen-server-openapi-original.json
  type: http
slug: oxen-authentication
source_filename: oxen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/oxen-hub-api-openapi-original.json, openapi/oxen-server-openapi-original.json\ndocs: https://docs.oxen.ai/getting-started/inference\nsummary:\n  types:\n  - http\n  model: >-\n    Oxen.ai authenticates every API request with a personal API key sent as an\n    HTTP Bearer token: `Authorization: Bearer $OXEN_API_KEY`. Keys are created in\n    account settings (https://www.oxen.ai/settings) and used identically by the\n    Hub AI/fine-tuning API, the data-version-control server API, the Python SDK\n    (oxenai), and the oxen CLI (`oxen config --auth hub.oxen.ai $TOKEN`). No OAuth\n    2.0 authorization-code / scope surface is published.\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API key. Header `Authorization: Bearer <OXEN_API_KEY>`. Same key across\n    inference, fine-tuning, and version-control endpoints.\n  sources:\n  - openapi/oxen-hub-api-openapi-original.json\n\
  \  - openapi/oxen-server-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/authentication/oxen-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Version Control
- Machine Learning
- Artificial Intelligence
- Fine-Tuning
- Inference
- Datasets
- MLOps
- Large Language Models
- Model Deployment
- Developer Tools
- Version Control
---
