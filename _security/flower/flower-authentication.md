---
api_key_in:
- sdk-attribute
auth_types:
- apiKey
description: Authentication across Flower Labs' two surfaces. There is no first-party OpenAPI in the repo, so this profile is derived from the official docs rather than a spec. Flower Intelligence's confidential remote-compute service authenticates with an API key; the Flower framework's hosted control plane (SuperLink / SuperGrid) authenticates via `flwr login`.
kind: authentication
layout: security
method: searched
name: Flower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flower secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flower
provider_slug: flower
scheme_count: 2
schemes:
- detail: Remote confidential compute is disabled by default. Callers enable it by setting `remoteHandoff = true` and supplying `apiKey = "YOUR_API_KEY"` on the Flower Intelligence singleton. API keys are issued via https://flower.ai/intelligence.
  docs: https://flower.ai/docs/intelligence/
  in: sdk-attribute
  name: FlowerIntelligenceApiKey
  sources:
  - docs
  type: apiKey
- detail: The Flower framework control plane is accessed after `flwr login` against a SuperLink / SuperGrid; connections are managed with `flwr config list`.
  docs: https://flower.ai/docs/framework/ref-api-cli.html
  in: cli
  name: SuperLinkLogin
  sources:
  - docs
  type: session
slug: flower-authentication
source_filename: flower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://flower.ai/docs/intelligence/ + https://flower.ai/docs/framework/ref-api-cli.html\ndescription: >-\n  Authentication across Flower Labs' two surfaces. There is no first-party\n  OpenAPI in the repo, so this profile is derived from the official docs rather\n  than a spec. Flower Intelligence's confidential remote-compute service\n  authenticates with an API key; the Flower framework's hosted control plane\n  (SuperLink / SuperGrid) authenticates via `flwr login`.\nsummary:\n  types: [apiKey]\n  api_key_in: [sdk-attribute]\n  oauth2_flows: []\nschemes:\n  - name: FlowerIntelligenceApiKey\n    type: apiKey\n    in: sdk-attribute\n    detail: >-\n      Remote confidential compute is disabled by default. Callers enable it by\n      setting `remoteHandoff = true` and supplying `apiKey = \"YOUR_API_KEY\"` on\n      the Flower Intelligence singleton. API keys are issued via\n      https://flower.ai/intelligence.\n    docs: https://flower.ai/docs/intelligence/\n\
  \    sources: [docs]\n  - name: SuperLinkLogin\n    type: session\n    in: cli\n    detail: >-\n      The Flower framework control plane is accessed after `flwr login` against\n      a SuperLink / SuperGrid; connections are managed with `flwr config list`.\n    docs: https://flower.ai/docs/framework/ref-api-cli.html\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flower/refs/heads/main/authentication/flower-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Federated Learning
- Federated AI
- Machine Learning
- Artificial Intelligence
- Privacy
- SDK
- On-Device AI
- Confidential Computing
- Open Source
---
