---
api_key_in:
- header
- query
api_specs:
- filename: jupyter-notebook-rest-api-openapi.yml
  format: yaml
  label: Jupyter Notebook REST API
  slug: jupyter-notebook-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-rest-api-openapi.yml
- filename: jupyter-kernel-gateway-api-openapi.yml
  format: yaml
  label: Jupyter Kernel Gateway API
  slug: jupyter-kernel-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-kernel-gateway-api-openapi.yml
- filename: jupyterhub-rest-api-openapi.yml
  format: yaml
  label: JupyterHub REST API
  slug: jupyterhub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyterhub-rest-api-openapi.yml
- filename: jupyter-kernel-messaging-asyncapi.yml
  format: yaml
  label: Jupyter Kernel Messaging Protocol
  slug: jupyter-kernel-messaging
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/asyncapi/jupyter-kernel-messaging-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jupyter Notebook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jupyter Notebook secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jupyter Notebook
provider_slug: jupyter-notebook
scheme_count: 3
schemes:
- description: Authentication token configured via KG_AUTH_TOKEN. Passed as 'token <token_value>' in the Authorization header.
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/jupyter-kernel-gateway-api-openapi.yml
  - openapi/jupyter-notebook-rest-api-openapi.yml
  - openapi/jupyterhub-rest-api-openapi.yml
  type: apiKey
- description: Authentication token passed as a query parameter.
  in: query
  name: tokenQuery
  parameter: token
  sources:
  - openapi/jupyter-kernel-gateway-api-openapi.yml
  - openapi/jupyter-notebook-rest-api-openapi.yml
  type: apiKey
- description: OAuth2 bearer token.
  name: oAuthToken
  scheme: bearer
  sources:
  - openapi/jupyterhub-rest-api-openapi.yml
  type: http
slug: jupyter-notebook-authentication
source_filename: jupyter-notebook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyter-kernel-gateway-api-openapi.yml, openapi/jupyter-notebook-rest-api-openapi.yml,\n  openapi/jupyterhub-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authentication token configured via KG_AUTH_TOKEN. Passed as 'token <token_value>'\n    in the Authorization header.\n  sources:\n  - openapi/jupyter-kernel-gateway-api-openapi.yml\n  - openapi/jupyter-notebook-rest-api-openapi.yml\n  - openapi/jupyterhub-rest-api-openapi.yml\n- name: tokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: Authentication token passed as a query parameter.\n  sources:\n  - openapi/jupyter-kernel-gateway-api-openapi.yml\n  - openapi/jupyter-notebook-rest-api-openapi.yml\n- name: oAuthToken\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token.\n  sources:\n\
  \  - openapi/jupyterhub-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/authentication/jupyter-notebook-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Data Science
- Interactive Computing
- Jupyter
- Machine Learning
- Notebooks
- Python
---
