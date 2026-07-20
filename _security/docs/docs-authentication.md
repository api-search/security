---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Docs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infini-AI (无问芯穹) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infini-AI (无问芯穹)
provider_slug: docs
scheme_count: 1
schemes:
- evidence:
  - POST /maas/v1/chat/completions with no token -> 401 {"code":60000,"msg":"Wrong Bearer Token or Token is nil"}
  - POST /maas/v1/chat/completions with bad token -> {"code":10009,"msg":"请使用正确的api key进行请求"}
  format: Bearer <API_KEY>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - live-probe https://cloud.infini-ai.com/maas/v1
  type: http
slug: docs-authentication
source_filename: docs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cloud.infini-ai.com/fundamentals/tenant/iam-credentials-api-key.html\ndocs: https://cloud.infini-ai.com/fundamentals/tenant/iam-credentials-api-key.html\nprovider: Infini-AI (无问芯穹) GenStudio\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  notes: >-\n    The GenStudio large-model service (MaaS) is OpenAI-compatible and authenticates\n    with a tenant-managed API Key passed as a Bearer token in the Authorization\n    header. Confirmed by live probe of the /maas/v1 endpoints (missing/invalid\n    tokens return the provider error envelope).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API_KEY>'\n  sources: [live-probe https://cloud.infini-ai.com/maas/v1]\n  evidence:\n  - 'POST /maas/v1/chat/completions with no token -> 401 {\"code\":60000,\"msg\":\"Wrong Bearer Token or Token is nil\"}'\n  - 'POST /maas/v1/chat/completions\
  \ with bad token -> {\"code\":10009,\"msg\":\"请使用正确的api key进行请求\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docs/refs/heads/main/authentication/docs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Model as a Service
- Inference
- ComfyUI
- Agents
- AGI Compute
- OpenAI-Compatible
---
