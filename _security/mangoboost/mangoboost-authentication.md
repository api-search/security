---
api_key_in: []
auth_types: []
description: MangoBoost has no hosted, credentialed API. Every surface is deployed inside the customer's own infrastructure, so authentication is a deployment concern rather than an API concern. The three credentials that do exist are for pulling assets (Hugging Face, container registry) and for activating the commercial license — not for calling the API. There is no API-key issuance, no OAuth, no OIDC, and no token endpoint anywhere on the MangoBoost surface.
kind: authentication
layout: security
method: searched
name: Mangoboost Authentication
name_suffix: Authentication
oauth_flows: []
overview: MangoBoost declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MangoBoost
provider_slug: mangoboost
scheme_count: 0
schemes: []
slug: mangoboost-authentication
source_filename: mangoboost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://llmboost.mangoboost.io/docs/features/openai-api\ndocs: https://llmboost.mangoboost.io/docs/running/lbh\nname: MangoBoost authentication and access model\ndescription: >-\n  MangoBoost has no hosted, credentialed API. Every surface is deployed inside the\n  customer's own infrastructure, so authentication is a deployment concern rather than an\n  API concern. The three credentials that do exist are for pulling assets (Hugging Face,\n  container registry) and for activating the commercial license — not for calling the API.\n  There is no API-key issuance, no OAuth, no OIDC, and no token endpoint anywhere on the\n  MangoBoost surface.\n\nsurfaces:\n  - api: Mango LLMBoost Inference Server API\n    transport: HTTP/1.1 REST on :8000 (default)\n    security_schemes: []\n    model: none-by-default\n    detail: >-\n      \"Drop the Authorization header for local serving, or put LLMBoost behind your own\n      gateway for auth.\"\
  \ Vendor examples set api_key=\"not-needed\". The OpenAI client\n      requires an api_key value, so any non-empty string works; the server does not\n      validate it.\n    recommendation: >-\n      Because the server ships with no authentication, network placement IS the access\n      control. Bind it to a private interface and front it with your own gateway (mTLS,\n      API keys, OAuth) before any non-loopback exposure.\n    url: https://llmboost.mangoboost.io/docs/features/openai-api\n\n  - api: Mango SDK Device API (libmango)\n    transport: In-process C/C++ library against a local PCIe device\n    security_schemes: []\n    model: os-privilege\n    detail: >-\n      Access is governed by Linux privileges on the device — mango-ctl and mango-smi\n      examples require sudo, and the container needs /dev/kfd and /dev/dri access for the\n      GPU path. There is no network authentication layer.\n    url: https://sdk.mangoboost.io/docs/api/\n\n  - api: Mango OPI Storage Bridge gRPC API\n\
  \    transport: gRPC on :50051 (HTTP gateway on :8082)\n    security_schemes: []\n    model: network-scoped\n    detail: >-\n      The vendor guide calls the bridge over plaintext gRPC with grpc_cli against\n      127.0.0.1:50051 or the DPU SoC address (192.168.1.2:50051), and notes that \"OPI API\n      calls can be made from any server with the same network as the DPU SoC.\" No TLS,\n      token or per-call credential is documented — the management network is the boundary.\n    url: https://sdk.mangoboost.io/docs/guide/docs_opi/guide\n\ncredentials:\n  - name: HF_TOKEN\n    kind: bearer-token\n    purpose: Hugging Face token for downloading gated or private model weights. Forwarded into the container.\n    obtained: hf auth login, or export HF_TOKEN=...\n    scope_of_use: model download only — never sent to the LLMBoost API.\n    url: https://llmboost.mangoboost.io/docs/quickstart\n\n  - name: container registry login\n    kind: registry-credential\n    purpose: Pull the LLMBoost server\
  \ image.\n    obtained: >-\n      Provisioned by MangoBoost — email contact@mangoboost.io with your Docker Hub\n      username to be invited to the LLMBoost image registry, then `docker login`.\n    url: https://llmboost.mangoboost.io/docs/running/lbh\n\n  - name: LLMBoost license\n    kind: license-file\n    default_path: $LBH_HOME/license.skm\n    purpose: Activates the licensed LLMBoost optimizations.\n    detail: >-\n      \"LLMBoost activates a license on first start (a free trial is provisioned\n      automatically) and then serves locally. Keep the host online for first activation.\"\n      Imported/validated with `lbh login`. Enterprise seats and offline licensing are\n      handled through mangoboost.io/contact.\n    url: https://llmboost.mangoboost.io/docs/running/configuration\n\nnot_present:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - api-key-issuance\n  - scopes-or-permissions-model\n\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n    - url: https://llmboost.mangoboost.io/docs/features/openai-api\n\
  \      http_status: 200\n    - url: https://llmboost.mangoboost.io/docs/running/configuration\n      http_status: 200\n    - url: https://sdk.mangoboost.io/docs/guide/docs_opi/guide\n      http_status: 200\n    - url: https://www.mangoboost.io/.well-known/openid-configuration\n      http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangoboost/refs/heads/main/authentication/mangoboost-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Infrastructure
- Data-Center
- Semiconductors
- Hardware
- Storage
- Networking
- Inference
- GPU
- DPU
---
