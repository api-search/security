---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Digitalgenius Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigitalGenius secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DigitalGenius
provider_slug: digitalgenius
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication using an encoded token built from an API key and secret created in the DigitalGenius Dashboard. For the MCP server and HTTP API, the encoded token is passed as `Authorization: Basic {{AUTH_TOKEN}}`. API keys are created in the Dashboard with a selectable Access Type (e.g. "All").'
  header: 'Authorization: Basic {{AUTH_TOKEN}}'
  name: basicAuth
  scheme: basic
  token_creation: Dashboard -> create API key (name + Access Type) -> "Copy Encoded Token".
  type: http
slug: digitalgenius-authentication
source_filename: digitalgenius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.digitalgenius.com/docs/create-basic-token\ndocs: https://docs.digitalgenius.com/docs/create-basic-token\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  identity_provider: Auth0\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using an encoded token built from an API key and\n    secret created in the DigitalGenius Dashboard. For the MCP server and HTTP API,\n    the encoded token is passed as `Authorization: Basic {{AUTH_TOKEN}}`. API keys\n    are created in the Dashboard with a selectable Access Type (e.g. \"All\").\n  header: 'Authorization: Basic {{AUTH_TOKEN}}'\n  token_creation: >-\n    Dashboard -> create API key (name + Access Type) -> \"Copy Encoded Token\".\nplatform_identity:\n  provider: Auth0\n  evidence: https://status.digitalgenius.com/\n  components:\n  - User Authentication\n  - Machine-to-Machine Authentication\n  - Multi-factor\
  \ Authentication\n  - Management API\n  note: >-\n    The DigitalGenius platform (Dashboard, M2M) is fronted by Auth0 per the public\n    status page. Programmatic API/MCP access uses the Basic encoded token above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitalgenius/refs/heads/main/authentication/digitalgenius-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Service
- Ecommerce
- Artificial Intelligence
- AI Agents
- Conversational AI
- Customer Support Automation
- Retail
- MCP
---
