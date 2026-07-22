---
api_key_in:
- config
auth_types:
- apiKey
description: Qwak (JFrog ML) platform authentication. Access is via a Qwak Service API Key. The `qwak` CLI persists the key locally with `qwak configure --api-key <KEY>`; the same key authenticates the Python/Go SDKs and CI runners (verified in the public qwak-ai build-action and deploy-action, which pass the key as a repository secret to `qwak configure --api-key $QWAK_API_KEY`). No standalone public OpenAPI declares the security schemes, so this profile is captured by search rather than derived from a spec.
kind: authentication
layout: security
method: searched
name: Qwak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwak secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qwak
provider_slug: qwak
scheme_count: 1
schemes:
- description: Service API Key issued from the Qwak/JFrog ML console. Applied via `qwak configure --api-key`, then used by the SDKs and CLI to authenticate build, deploy, and inference calls.
  in: config
  name: QwakServiceApiKey
  sources:
  - https://github.com/qwak-ai/build-action
  - https://github.com/qwak-ai/deploy-action
  type: apiKey
slug: qwak-authentication
source_filename: qwak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qwak.com/docs\ndocs: https://docs.qwak.com/docs\ndescription: >-\n  Qwak (JFrog ML) platform authentication. Access is via a Qwak Service API Key.\n  The `qwak` CLI persists the key locally with `qwak configure --api-key <KEY>`;\n  the same key authenticates the Python/Go SDKs and CI runners (verified in the\n  public qwak-ai build-action and deploy-action, which pass the key as a\n  repository secret to `qwak configure --api-key $QWAK_API_KEY`). No standalone\n  public OpenAPI declares the security schemes, so this profile is captured by\n  search rather than derived from a spec.\nsummary:\n  types: [apiKey]\n  api_key_in: [config]\n  oauth2_flows: []\nschemes:\n  - name: QwakServiceApiKey\n    type: apiKey\n    in: config\n    description: >-\n      Service API Key issued from the Qwak/JFrog ML console. Applied via\n      `qwak configure --api-key`, then used by the SDKs and CLI to authenticate\n      build,\
  \ deploy, and inference calls.\n    sources:\n      - https://github.com/qwak-ai/build-action\n      - https://github.com/qwak-ai/deploy-action\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwak/refs/heads/main/authentication/qwak-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Machine Learning
- MLOps
- LLMOps
- Feature Store
- Model Deployment
- Model Monitoring
- Developer Tools
---
