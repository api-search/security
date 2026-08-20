---
api_key_in: []
api_specs:
- filename: furiosa-predict-v2.yaml
  format: yaml
  label: Furiosa Model Server - Predict API (KServe v2)
  slug: furiosa-server-predict-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/openapi/furiosa-predict-v2.yaml
- filename: furiosa-model-repository-v2.yaml
  format: yaml
  label: Furiosa Model Server - Model Repository API
  slug: furiosa-model-repository-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/openapi/furiosa-model-repository-v2.yaml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Furiosa Authentication
name_suffix: Authentication
oauth_flows: []
overview: FuriosaAI declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: FuriosaAI
provider_slug: furiosa
scheme_count: 0
schemes: []
slug: furiosa-authentication
source_filename: furiosa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: >-\n  https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html,\n  https://developer.furiosa.ai/latest/en/overview/roadmap.html,\n  https://github.com/furiosa-ai/furiosa-sdk/blob/main/python/furiosa-server/README.md\ndocs: https://developer.furiosa.ai/latest/en/furiosa_llm/furiosa-llm-serve.html\nsummary: >-\n  FuriosaAI operates no hosted API, so there is no FuriosaAI-issued credential anywhere in this\n  profile. Both HTTP surfaces are software the customer runs on their own machines, and each one\n  authenticates (or does not) on the customer's terms. That is the honest shape of the auth\n  story here, and it is why no OAuth scopes artifact exists.\nsurfaces:\n  - api: furiosa-llm-openai-server\n    name: Furiosa-LLM OpenAI-Compatible Server\n    schemes:\n      - type: http\n        scheme: bearer\n        name: OpenAI-style API key\n        header: 'Authorization: Bearer <key>'\n        required: false\n\
  \        issued_by: the operator of the server, not FuriosaAI\n        evidence: >-\n          The roadmap records \"✅ API Key based authentication support\" delivered in the\n          2025 Q3-Q4 train. Every code example in the serving docs sends\n          `api_key = os.getenv(\"OPENAI_API_KEY\", \"EMPTY\")`, and the raw curl example sends no\n          Authorization header at all - i.e. the server runs unauthenticated by default and the\n          key is opt-in, set by whoever launches `furiosa-llm serve`.\n        note: >-\n          The docs do not publish the server flag that enables it or the failure status code.\n          Establishing those requires reading `furiosa-llm serve --help` on an installed build.\n    model_value_ignored: >-\n      Worth recording as an auth-adjacent quirk: the `model` field is required by OpenAI clients\n      but IGNORED by the server, because one `furiosa-llm serve` process hosts exactly one model.\n      Callers should read the real id from GET\
  \ /v1/models rather than assume routing by name.\n  - api: furiosa-server-predict-v2\n    name: Furiosa Model Server (KServe v2 Predict + Triton Model Repository)\n    schemes: []\n    security_schemes_in_spec: false\n    evidence: >-\n      Neither openapi/furiosa-predict-v2.yaml nor openapi/furiosa-model-repository-v2.yaml\n      declares a `securitySchemes` block or any `security` requirement, and the furiosa-server\n      README lists \"Authentication support\" as an UNCHECKED roadmap item. The server is designed\n      to sit behind the customer's own ingress/mesh.\n    note: >-\n      This is a real finding, not an omission on our side: the model-repository surface exposes\n      unauthenticated load/unload of arbitrary models from the repository root, so it must never\n      be exposed outside a trusted network.\noauth: false\noauth_note: >-\n  No OAuth 2.0 or OpenID Connect anywhere - no authorization server, no scopes, no\n  /.well-known/oauth-authorization-server (probed 404\
  \ on all hosts, see well-known/).\n  scopes/ is therefore intentionally absent rather than empty.\nmtls: false\nscheme_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/authentication/furiosa-authentication.yml
summary_line: 0 schemes
tags:
- Artificial Intelligence
- Machine-Learning
- Inference
- Semiconductors
- NPU
- Hardware
- LLM
- Model Serving
- Kubernetes
- Developer Tools
- Compute
- Infrastructure
---
