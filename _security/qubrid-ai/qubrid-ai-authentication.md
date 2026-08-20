---
api_key_in: []
api_specs:
- filename: qubrid-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Qubrid AI Chat Completions API
  slug: qubrid-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-chat-completions-api-openapi.yml
- filename: qubrid-ai-datasets-api-openapi.yml
  format: yaml
  label: Qubrid AI Datasets API
  slug: qubrid-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-datasets-api-openapi.yml
- filename: qubrid-ai-documents-api-openapi.yml
  format: yaml
  label: Qubrid AI Documents API
  slug: qubrid-ai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-documents-api-openapi.yml
- filename: qubrid-ai-embeddings-api-openapi.yml
  format: yaml
  label: Qubrid AI Embeddings API
  slug: qubrid-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-embeddings-api-openapi.yml
- filename: qubrid-ai-fine-tuned-models-api-openapi.yml
  format: yaml
  label: Qubrid AI Fine-Tuned Models API
  slug: qubrid-ai-fine-tuned-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-fine-tuned-models-api-openapi.yml
- filename: qubrid-ai-fine-tuning-jobs-api-openapi.yml
  format: yaml
  label: Qubrid AI Fine-Tuning Jobs API
  slug: qubrid-ai-fine-tuning-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-fine-tuning-jobs-api-openapi.yml
- filename: qubrid-ai-gpu-catalog-api-openapi.yml
  format: yaml
  label: Qubrid AI GPU Catalog API
  slug: qubrid-ai-gpu-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-gpu-catalog-api-openapi.yml
- filename: qubrid-ai-instances-api-openapi.yml
  format: yaml
  label: Qubrid AI Instances API
  slug: qubrid-ai-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-instances-api-openapi.yml
- filename: qubrid-ai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Qubrid AI Knowledge Bases API
  slug: qubrid-ai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-knowledge-bases-api-openapi.yml
- filename: qubrid-ai-models-api-openapi.yml
  format: yaml
  label: Qubrid AI Models API
  slug: qubrid-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-models-api-openapi.yml
- filename: qubrid-ai-rag-queries-api-openapi.yml
  format: yaml
  label: Qubrid AI RAG Queries API
  slug: qubrid-ai-rag-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-rag-queries-api-openapi.yml
- filename: qubrid-ai-ssh-keys-api-openapi.yml
  format: yaml
  label: Qubrid AI SSH Keys API
  slug: qubrid-ai-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-ssh-keys-api-openapi.yml
- filename: qubrid-ai-templates-api-openapi.yml
  format: yaml
  label: Qubrid AI Templates API
  slug: qubrid-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-templates-api-openapi.yml
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
- Machine-Learning
- NVIDIA
- Serverless
---
