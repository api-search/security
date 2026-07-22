---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vianai Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vianai Systems secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vianai Systems
provider_slug: vianai-systems
scheme_count: 2
schemes:
- description: 'Access token returned by POST /v1/user/login (field access_token). Sent as "Authorization: <access_token>" on subsequent REST and SDK requests.'
  logout_endpoint: /v1/user/logout
  name: bearerToken
  scheme: bearer
  sources:
  - https://docs.vian.ai/5.0-r2/api-quickstart.html
  token_endpoint: /v1/user/login
  type: http
- description: Per-user API key managed via /v1/user/api-key; used as the x-api-key header (e.g. to fetch the vianops-client SDK/CLI wheel from webservices/<host>/v1/sdk).
  in: header
  name: apiKey
  name_param: x-api-key
  sources:
  - https://docs.vian.ai/5.0-r2/vianctl.html
  type: apiKey
slug: vianai-systems-authentication
source_filename: vianai-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vian.ai/5.0-r2/api-quickstart.html\ndocs: https://docs.vian.ai/5.0-r2/api-quickstart.html\nsummary:\n  types:\n  - http\n  - apiKey\n  http_schemes:\n  - bearer\n  api_key_in:\n  - header\n  notes: >-\n    Most hila REST and SDK calls require an authorization bearer token. A token is\n    obtained by POSTing username/password to /v1/user/login and reading access_token\n    from the response; it is then sent on the Authorization header of subsequent calls.\n    A long-lived API key (x-api-key header) is also issued via /v1/user/api-key and is\n    used to download the SDK/CLI wheel from the deployment.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Access token returned by POST /v1/user/login (field access_token). Sent as\n    \"Authorization: <access_token>\" on subsequent REST and SDK requests.\n  token_endpoint: /v1/user/login\n  logout_endpoint: /v1/user/logout\n  sources:\n\
  \  - https://docs.vian.ai/5.0-r2/api-quickstart.html\n- name: apiKey\n  type: apiKey\n  in: header\n  name_param: x-api-key\n  description: >-\n    Per-user API key managed via /v1/user/api-key; used as the x-api-key header (e.g.\n    to fetch the vianops-client SDK/CLI wheel from webservices/<host>/v1/sdk).\n  sources:\n  - https://docs.vian.ai/5.0-r2/vianctl.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vianai-systems/refs/heads/main/authentication/vianai-systems-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- MLOps
- Model Monitoring
- Analytics
- Generative AI
- Observability
- Conversational Analytics
---
