---
api_key_in:
- header
api_specs:
- filename: armada-orchestrator-openapi-original.yml
  format: yaml
  label: Armada Bridge Orchestrator API
  slug: armada-bridge-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armada/refs/heads/main/openapi/armada-orchestrator-openapi-original.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Armada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Armada secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Armada
provider_slug: armada
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'Orchestrator API: JWT Bearer token in the Authorization header, issued by the platform auth middleware.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/armada-orchestrator-openapi-original.yml
  type: http
- description: 'Bridge AI Studio Model-as-a-Service: an API key presented as a Bearer token (Authorization: Bearer $API_KEY). Keys are created and revoked in AI Studio Settings and shown once at creation.'
  name: modelServiceApiKey
  scheme: bearer
  sources:
  - https://docs.armada.ai/bridge/tenant-guide/ai-studio/model-as-a-service/api-key
  type: http
- description: Console/UI sign-in (console.armada.ai, Atlas / Armada Edge Platform) is OIDC, backed by Keycloak.
  name: consoleOIDC
  sources:
  - https://console.armada.ai/
  type: openIdConnect
slug: armada-authentication
source_filename: armada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/armada-orchestrator-openapi-original.yml\ndocs: https://docs.armada.ai/bridge/tenant-guide/ai-studio/model-as-a-service/api-key\nsummary:\n  types:\n  - http\n  - openIdConnect\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Orchestrator API: JWT Bearer token in the Authorization header, issued by the\n    platform auth middleware.\n  sources:\n  - openapi/armada-orchestrator-openapi-original.yml\n- name: modelServiceApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Bridge AI Studio Model-as-a-Service: an API key presented as a Bearer token\n    (Authorization: Bearer $API_KEY). Keys are created and revoked in AI Studio\n    Settings and shown once at creation.\n  sources:\n  - https://docs.armada.ai/bridge/tenant-guide/ai-studio/model-as-a-service/api-key\n- name: consoleOIDC\n  type: openIdConnect\n\
  \  description: >-\n    Console/UI sign-in (console.armada.ai, Atlas / Armada Edge Platform) is OIDC,\n    backed by Keycloak.\n  sources:\n  - https://console.armada.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armada/refs/heads/main/authentication/armada-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Company
- Edge Computing
- GPU Cloud
- Infrastructure
- Artificial Intelligence
- Kubernetes
- Bare Metal
- IoT
- Orchestration
- Sovereign Cloud
---
