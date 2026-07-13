---
api_key_in:
- header
api_specs:
- filename: jupyterlab-server-rest-api-openapi.yml
  format: yaml
  label: JupyterLab Server REST API
  slug: jupyterlab-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterlab/refs/heads/main/openapi/jupyterlab-server-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jupyterlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: JupyterLab secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JupyterLab
provider_slug: jupyterlab
scheme_count: 2
schemes:
- description: 'Token-based authentication. Use the form: Authorization: token <token>'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/jupyterlab-server-rest-api-openapi.yml
  type: apiKey
- description: XSRF token required for browser-based requests.
  in: header
  name: xsrf
  parameter: X-XSRFToken
  sources:
  - openapi/jupyterlab-server-rest-api-openapi.yml
  type: apiKey
slug: jupyterlab-authentication
source_filename: jupyterlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyterlab-server-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Use the form: Authorization: token <token>'\n  sources:\n  - openapi/jupyterlab-server-rest-api-openapi.yml\n- name: xsrf\n  type: apiKey\n  in: header\n  parameter: X-XSRFToken\n  description: XSRF token required for browser-based requests.\n  sources:\n  - openapi/jupyterlab-server-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyterlab/refs/heads/main/authentication/jupyterlab-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Science
- Extensions
- IDE
- Interactive Computing
- Notebooks
- Python
---
