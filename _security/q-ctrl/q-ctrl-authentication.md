---
api_key_in:
- account-issued token
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Q Ctrl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Q Ctrl secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Q Ctrl
provider_slug: q-ctrl
scheme_count: 1
schemes:
- description: An account-issued API key (managed at https://accounts.q-ctrl.com) is used by the Q-CTRL Python clients to authenticate. Once authenticated, requests are made to the Q-CTRL cloud GraphQL endpoint.
  managed_at: https://accounts.q-ctrl.com/
  name: qctrl-api-key
  sources:
  - docs.q-ctrl.com
  type: apiKey
slug: q-ctrl-authentication
source_filename: q-ctrl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.q-ctrl.com/boulder-opal/get-started\nnote: >-\n  Q-CTRL does not publish a public OpenAPI/Swagger spec. The cloud is reached\n  through the official Python clients (boulder-opal, fire-opal), which\n  authenticate the caller against the Q-CTRL account service and then call the\n  hosted GraphQL API at https://api.q-ctrl.com/graphql.\nsummary:\n  types: [apiKey]\n  api_key_in: [account-issued token]\n  oauth2_flows: []\nschemes:\n- name: qctrl-api-key\n  type: apiKey\n  description: >-\n    An account-issued API key (managed at https://accounts.q-ctrl.com) is used\n    by the Q-CTRL Python clients to authenticate. Once authenticated, requests\n    are made to the Q-CTRL cloud GraphQL endpoint.\n  managed_at: https://accounts.q-ctrl.com/\n  sources: [docs.q-ctrl.com]\nendpoints:\n  graphql: https://api.q-ctrl.com/graphql\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/q-ctrl/refs/heads/main/authentication/q-ctrl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Quantum Computing
- Quantum Control
- Quantum Sensing
- Error Suppression
- Developer Tools
- SDK
- GraphQL API
---
