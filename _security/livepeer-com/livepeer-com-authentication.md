---
api_key_in: []
api_specs:
- filename: livepeer-studio-openapi.yml
  format: yaml
  label: Livepeer Studio API
  slug: studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-studio-openapi.yml
- filename: livepeer-ai-worker-openapi.yml
  format: yaml
  label: Livepeer AI Network
  slug: ai-network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-ai-worker-openapi.yml
- filename: livepeer-cli-http-openapi.yml
  format: yaml
  label: Livepeer Node CLI HTTP API
  slug: cli-http
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-cli-http-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Livepeer Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Livepeer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Livepeer
provider_slug: livepeer-com
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/livepeer-ai-worker-openapi.yml
  - openapi/livepeer-gateway-openapi.yml
  - openapi/livepeer-studio-openapi.yml
  type: http
slug: livepeer-com-authentication
source_filename: livepeer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/livepeer-ai-worker-openapi.yml, openapi/livepeer-gateway-openapi.yml, openapi/livepeer-studio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/livepeer-ai-worker-openapi.yml\n  - openapi/livepeer-gateway-openapi.yml\n  - openapi/livepeer-studio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/authentication/livepeer-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Live Streaming
- Video On Demand
- AI Video
- Decentralized Compute
- GPU Network
- Ethereum
- Arbitrum
- Web3
---
