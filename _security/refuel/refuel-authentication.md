---
api_key_in:
- env
- sdk-option
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Refuel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refuel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Refuel
provider_slug: refuel
scheme_count: 1
schemes:
- description: API key issued per team/account. Supplied via the REFUEL_API_KEY environment variable (picked up automatically by refuel.init()) or passed as the `api_key` option to refuel.init(**options). Used to authenticate all requests to the Refuel API server.
  in: env
  name: apiKey
  parameter: REFUEL_API_KEY
  sources:
  - https://docs.refuel.ai/sdk/python
  - https://docs.refuel.ai/sdk/javascript
  type: apiKey
slug: refuel-authentication
source_filename: refuel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.refuel.ai/sdk/python\ndocs: https://docs.refuel.ai/sdk/python\nsummary:\n  types: [apiKey]\n  api_key_in: [env, sdk-option]\n  oauth2_flows: []\n  notes: >-\n    Refuel Cloud authenticates every request with an API key. The SDKs read it\n    from the REFUEL_API_KEY environment variable, or accept it as an `api_key`\n    initialization option. A `project` selector scopes all downstream calls\n    (datasets, tasks, etc.) to a single project in the team account.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: env\n  parameter: REFUEL_API_KEY\n  description: >-\n    API key issued per team/account. Supplied via the REFUEL_API_KEY environment\n    variable (picked up automatically by refuel.init()) or passed as the\n    `api_key` option to refuel.init(**options). Used to authenticate all\n    requests to the Refuel API server.\n  sources:\n  - https://docs.refuel.ai/sdk/python\n  - https://docs.refuel.ai/sdk/javascript\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuel/refs/heads/main/authentication/refuel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Labeling
- Machine Learning
- LLM
- Data Enrichment
- Artificial Intelligence
- Data Transformation
- MLOps
- SDK
---
