---
api_key_in:
- client
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Onepot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onepot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onepot
provider_slug: onepot
scheme_count: 1
schemes:
- description: API key supplied to the onepot Python client constructor (Client(api_key=...)) and sent to the REST API on each call. Obtained via "Request API access" on the API docs page.
  in: client
  name: apiKey
  sources:
  - https://www.onepot.ai/api
  type: apiKey
slug: onepot-authentication
source_filename: onepot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.onepot.ai/api\ndocs: https://www.onepot.ai/api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - client\n  oauth2_flows: []\n  access: gated\n  notes: >-\n    Access is gated behind \"Request API access\". The onepot Python client is\n    constructed with an API key (Client(api_key=\"your-api-key\")); the client\n    attaches the key to the underlying REST API requests. No OAuth2/OIDC surface\n    is documented; the public discovery well-known endpoints (openid-configuration,\n    oauth-authorization-server) return 404.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: client\n  description: >-\n    API key supplied to the onepot Python client constructor\n    (Client(api_key=...)) and sent to the REST API on each call. Obtained via\n    \"Request API access\" on the API docs page.\n  sources:\n  - https://www.onepot.ai/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onepot/refs/heads/main/authentication/onepot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Chemistry
- Cheminformatics
- Drug Discovery
- Small Molecule Synthesis
- Contract Research Organization
- Artificial Intelligence
- Machine Learning
- Lab Automation
- Life Sciences
- API
---
