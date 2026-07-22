---
api_key_in:
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Telekinesisai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telekinesis.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telekinesis.ai
provider_slug: telekinesisai
scheme_count: 1
schemes:
- description: An API key is created at https://platform.telekinesis.ai/api-keys and supplied to the SDK via the TELEKINESIS_API_KEY environment variable (or passed directly to the client). Used for cloud-hosted skill execution and Physical AI agent access.
  in: environment
  name: TelekinesisApiKey
  parameter: TELEKINESIS_API_KEY
  provisioning_url: https://platform.telekinesis.ai/api-keys
  sources:
  - docs.telekinesis.ai/getting-started/quickstart
  type: apiKey
slug: telekinesisai-authentication
source_filename: telekinesisai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.telekinesis.ai/getting-started/quickstart\ndocs: https://docs.telekinesis.ai/getting-started/quickstart\nnote: >-\n  Telekinesis does not publish an OpenAPI specification; this profile is\n  captured from the developer documentation. The Telekinesis SDK authenticates\n  with a personal API key created in the platform console.\nsummary:\n  types: [apiKey]\n  api_key_in: [environment]\nschemes:\n  - name: TelekinesisApiKey\n    type: apiKey\n    in: environment\n    parameter: TELEKINESIS_API_KEY\n    description: >-\n      An API key is created at https://platform.telekinesis.ai/api-keys and\n      supplied to the SDK via the TELEKINESIS_API_KEY environment variable\n      (or passed directly to the client). Used for cloud-hosted skill\n      execution and Physical AI agent access.\n    provisioning_url: https://platform.telekinesis.ai/api-keys\n    sources: [docs.telekinesis.ai/getting-started/quickstart]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telekinesisai/refs/heads/main/authentication/telekinesisai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Robotics
- Computer Vision
- Physical AI
- Industrial Automation
- Manufacturing Automation
- 6D Pose Estimation
- Motion Planning
- Reinforcement Learning
- Python SDK
- Embodied Intelligence
- Agents
---
