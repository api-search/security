---
api_key_in:
- header
api_specs:
- filename: jupyter-server-checkpoints-api-openapi.yml
  format: yaml
  label: Jupyter Server Checkpoints API
  slug: jupyter-server-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-checkpoints-api-openapi.yml
- filename: jupyter-server-config-api-openapi.yml
  format: yaml
  label: Jupyter Server Config API
  slug: jupyter-server-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-config-api-openapi.yml
- filename: jupyter-server-contents-api-openapi.yml
  format: yaml
  label: Jupyter Server Contents API
  slug: jupyter-server-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-contents-api-openapi.yml
- filename: jupyter-server-general-api-openapi.yml
  format: yaml
  label: Jupyter Server General API
  slug: jupyter-server-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-general-api-openapi.yml
- filename: jupyter-server-kernels-api-openapi.yml
  format: yaml
  label: Jupyter Server Kernels API
  slug: jupyter-server-kernels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-kernels-api-openapi.yml
- filename: jupyter-server-kernelspecs-api-openapi.yml
  format: yaml
  label: Jupyter Server Kernelspecs API
  slug: jupyter-server-kernelspecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-kernelspecs-api-openapi.yml
- filename: jupyter-server-sessions-api-openapi.yml
  format: yaml
  label: Jupyter Server Sessions API
  slug: jupyter-server-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-sessions-api-openapi.yml
- filename: jupyter-server-terminals-api-openapi.yml
  format: yaml
  label: Jupyter Server Terminals API
  slug: jupyter-server-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/openapi/jupyter-server-terminals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jupyter Server Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jupyter Server secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jupyter Server
provider_slug: jupyter-server
scheme_count: 2
schemes:
- description: 'Token-based authentication. Use the form: Authorization: token <token>'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/jupyter-server-rest-api-openapi.yml
  type: apiKey
- description: XSRF token required for browser-based requests.
  in: header
  name: xsrf
  parameter: X-XSRFToken
  sources:
  - openapi/jupyter-server-rest-api-openapi.yml
  type: apiKey
slug: jupyter-server-authentication
source_filename: jupyter-server-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyter-server-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Use the form: Authorization: token <token>'\n  sources:\n  - openapi/jupyter-server-rest-api-openapi.yml\n- name: xsrf\n  type: apiKey\n  in: header\n  parameter: X-XSRFToken\n  description: XSRF token required for browser-based requests.\n  sources:\n  - openapi/jupyter-server-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/authentication/jupyter-server-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Compute
- Interactive Computing
- Kernels
- Notebooks
- Portable
- Workbooks
---
