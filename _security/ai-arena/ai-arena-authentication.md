---
api_key_in:
- cli-token
auth_types:
- apiKey
description: Authentication profile for ArenaX Labs surfaces. The SAI research platform (competesai.com) CLI authenticates with a bearer API token obtained from account settings. The open-source RLMesh gRPC protocol intentionally leaves transport security and authentication out of scope (deployment concern), so it declares no built-in scheme.
kind: authentication
layout: security
method: searched
name: Ai Arena Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Arena secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AI Arena
provider_slug: ai-arena
scheme_count: 2
schemes:
- in: token
  mechanism: 'Bearer API token: `sai auth login --token YOUR_API_TOKEN` (token from account settings).'
  name: sai-api-token
  sources:
  - https://github.com/ArenaX-Labs/homebrew-tap/blob/main/sai.rb
  - https://github.com/ArenaX-Labs/scoop-bucket/blob/main/sai.json
  surface: SAI Platform (competesai.com)
  type: apiKey
- name: rlmesh-wire
  note: The 2026.06 workflow edition explicitly does not constrain transport security or authentication; those evolve freely at the deployment layer.
  sources:
  - https://docs.rlmesh.dev/en/v0.1.0-rc.2/compatibility/
  surface: RLMesh gRPC protocol (rlmesh-wire-v1)
  type: none
slug: ai-arena-authentication
source_filename: ai-arena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/ArenaX-Labs/homebrew-tap/blob/main/sai.rb\ndocs: https://competesai.com\ndescription: >-\n  Authentication profile for ArenaX Labs surfaces. The SAI research platform\n  (competesai.com) CLI authenticates with a bearer API token obtained from\n  account settings. The open-source RLMesh gRPC protocol intentionally leaves\n  transport security and authentication out of scope (deployment concern), so it\n  declares no built-in scheme.\nsummary:\n  types: [apiKey]\n  api_key_in: [cli-token]\n  oauth2_flows: []\nschemes:\n  - name: sai-api-token\n    surface: SAI Platform (competesai.com)\n    type: apiKey\n    in: token\n    mechanism: \"Bearer API token: `sai auth login --token YOUR_API_TOKEN` (token from account settings).\"\n    sources:\n      - https://github.com/ArenaX-Labs/homebrew-tap/blob/main/sai.rb\n      - https://github.com/ArenaX-Labs/scoop-bucket/blob/main/sai.json\n  - name: rlmesh-wire\n    surface:\
  \ RLMesh gRPC protocol (rlmesh-wire-v1)\n    type: none\n    note: >-\n      The 2026.06 workflow edition explicitly does not constrain transport\n      security or authentication; those evolve freely at the deployment layer.\n    sources:\n      - https://docs.rlmesh.dev/en/v0.1.0-rc.2/compatibility/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-arena/refs/heads/main/authentication/ai-arena-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Gaming
- Web3
- Artificial Intelligence
- Reinforcement Learning
- Machine Learning
- gRPC
- SDK
- Developer Tools
---
