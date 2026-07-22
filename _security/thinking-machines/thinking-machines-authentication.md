---
api_key_in: []
auth_types: []
description: The Tinker API and SDK authenticate with a single API key issued from the Tinker Console. The key is supplied to the SDK/CLI via the TINKER_API_KEY environment variable and is sent as a bearer credential to the service.
kind: authentication
layout: security
method: searched
name: Thinking Machines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thinking Machines declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Thinking Machines
provider_slug: thinking-machines
scheme_count: 1
schemes:
- description: Personal/organization API key obtained from the Tinker Console (https://tinker.thinkingmachines.ai/). Set as `export TINKER_API_KEY=...`; the Python SDK (import tinker) and the tinker CLI read it automatically.
  id: api_key
  in: env
  name: TINKER_API_KEY
  provisioning: https://tinker.thinkingmachines.ai/
  transport: bearer
  type: apiKey
slug: thinking-machines-authentication
source_filename: thinking-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: 2026-07-21\nmethod: searched\nsource: https://tinker-docs.thinkingmachines.ai/tinker/quickstart/\nname: Thinking Machines (Tinker) authentication\ndescription: >-\n  The Tinker API and SDK authenticate with a single API key issued from the\n  Tinker Console. The key is supplied to the SDK/CLI via the TINKER_API_KEY\n  environment variable and is sent as a bearer credential to the service.\nschemes:\n- id: api_key\n  type: apiKey\n  in: env\n  name: TINKER_API_KEY\n  transport: bearer\n  description: >-\n    Personal/organization API key obtained from the Tinker Console\n    (https://tinker.thinkingmachines.ai/). Set as `export TINKER_API_KEY=...`;\n    the Python SDK (import tinker) and the tinker CLI read it automatically.\n  provisioning: https://tinker.thinkingmachines.ai/\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: >-\n  Access control is enforced beyond authentication via a project-scoped\n  permission model (organizations, teams, projects,\
  \ sessions) documented at\n  https://tinker-docs.thinkingmachines.ai/tinker/data-model/. The SDK surfaces\n  AuthenticationError and PermissionDeniedError for credential/authorization\n  failures.\ndocs: https://tinker-docs.thinkingmachines.ai/tinker/quickstart/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinking-machines/refs/heads/main/authentication/thinking-machines-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- Fine-Tuning
- LLM
- Model Training
- Developer Tools
---
