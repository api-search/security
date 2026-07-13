---
api_key_in: []
api_specs:
- filename: qubrid-ai-inference-openapi.yml
  format: yaml
  label: Qubrid AI Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-inference-openapi.yml
- filename: qubrid-ai-compute-openapi.yml
  format: yaml
  label: Qubrid AI Compute API
  slug: compute
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-compute-openapi.yml
- filename: qubrid-ai-fine-tuning-openapi.yml
  format: yaml
  label: Qubrid AI Fine-Tuning API
  slug: fine-tuning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-fine-tuning-openapi.yml
- filename: qubrid-ai-rag-openapi.yml
  format: yaml
  label: Qubrid AI RAG API
  slug: rag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-rag-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qubrid Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qubrid AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qubrid AI
provider_slug: qubrid-ai
scheme_count: 1
schemes:
- bearerFormat: QUBRID_API_KEY
  description: Qubrid AI API key passed as a bearer token in the Authorization header. Obtain your API key from the Qubrid AI platform dashboard at https://platform.qubrid.com.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qubrid-ai-compute-openapi.yml
  - openapi/qubrid-ai-fine-tuning-openapi.yml
  - openapi/qubrid-ai-inference-openapi.yml
  - openapi/qubrid-ai-rag-openapi.yml
  type: http
slug: qubrid-ai-authentication
source_filename: qubrid-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qubrid-ai-compute-openapi.yml, openapi/qubrid-ai-fine-tuning-openapi.yml, openapi/qubrid-ai-inference-openapi.yml,\n  openapi/qubrid-ai-rag-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: QUBRID_API_KEY\n  description: Qubrid AI API key passed as a bearer token in the Authorization header. Obtain\n    your API key from the Qubrid AI platform dashboard at https://platform.qubrid.com.\n  sources:\n  - openapi/qubrid-ai-compute-openapi.yml\n  - openapi/qubrid-ai-fine-tuning-openapi.yml\n  - openapi/qubrid-ai-inference-openapi.yml\n  - openapi/qubrid-ai-rag-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/authentication/qubrid-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Cloud Computing
- GPU
- Inference
- Large Language Models
- Machine Learning
- NVIDIA
- Serverless
---
