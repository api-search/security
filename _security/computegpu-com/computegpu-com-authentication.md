---
anonymous_access: false
api_key_in: []
api_specs:
- filename: computegpu-com-gpu-api-openapi.yml
  format: yaml
  label: ComputeGpu Gpu API
  slug: computegpu-com-gpu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computegpu-com/openapi/computegpu-com-gpu-api-openapi.yml
- filename: computegpu-com-signup-api-openapi.yml
  format: yaml
  label: ComputeGpu Signup API
  slug: computegpu-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computegpu-com/openapi/computegpu-com-signup-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ComputeGpu Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComputeGpu secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ComputeGpu
provider_slug: computegpu-com
scheme_count: 3
schemes:
- description: GPU API key. Get one via POST /api/signup.
  header: 'Authorization: Bearer gpu_your_key'
  key_format: gpu_{tenantId}_{random}
  name: bearerAuth
  scheme: bearer
  scope: Account-wide (CLI login, REST API)
  sources:
  - openapi/computegpu-com-openapi.yml
  - https://computegpu.com/docs
  - https://computegpu.com/llms.txt
  type: http
- description: Per-rental key "(hex, no prefix)" returned when a GPU is rented; used only for the Ollama proxy at /api/v1/ollama/:rentalId/*. Not declared in the OpenAPI.
  name: rentalProxyKey
  scheme: bearer
  scope: Per-rental
  sources:
  - https://computegpu.com/docs
  type: http
- description: Dashboard session cookie; the docs show POST /auth/api-key and the Wallet API (/wallet/*) as "session auth required". Not declared in the OpenAPI and not probed.
  name: session
  sources:
  - https://computegpu.com/docs
  type: cookie
slug: computegpu-com-authentication
source_filename: computegpu-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://computegpu.com/docs\ndocs: https://computegpu.com/docs\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: GPU API key. Get one via POST /api/signup.\n  header: 'Authorization: Bearer gpu_your_key'\n  key_format: gpu_{tenantId}_{random}\n  scope: Account-wide (CLI login, REST API)\n  sources:\n  - openapi/computegpu-com-openapi.yml\n  - https://computegpu.com/docs\n  - https://computegpu.com/llms.txt\n- name: rentalProxyKey\n  type: http\n  scheme: bearer\n  description: Per-rental key \"(hex, no prefix)\" returned when a GPU is rented; used only for the Ollama proxy at /api/v1/ollama/:rentalId/*. Not declared in the OpenAPI.\n  scope: Per-rental\n  sources:\n  - https://computegpu.com/docs\n- name: session\n  type: cookie\n  description: Dashboard session cookie; the docs show POST /auth/api-key and the Wallet API (/wallet/*) as \"session auth required\". Not\
  \ declared in the OpenAPI and not probed.\n  sources:\n  - https://computegpu.com/docs\nkey_issuance:\n- CLI `computegpu signup you@co.com my-agent` (returns a gpu_ key instantly; CLI stores it in ~/.computegpu/config.json)\n- POST /api/signup (operationId agentSignup)\n- Dashboard Settings → API Keys\noauth: none documented\n"
source_yaml_url: https://artifacts.apis.io/computegpu-com/authentication/computegpu-com-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- GPU Cloud
- AI Infrastructure
- Compute
- Machine Learning
- Inference
- LLM
- MCP
- CLI
---
