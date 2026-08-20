---
api_key_in:
- header
- query
api_specs:
- filename: jupyter-kernel-messaging-asyncapi.yml
  format: yaml
  label: Jupyter Kernel Messaging Protocol
  slug: jupyter-kernel-messaging
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/asyncapi/jupyter-kernel-messaging-asyncapi.yml
- filename: jupyter-notebook-authorization-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Authorization API
  slug: jupyter-notebook-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-authorization-api-openapi.yml
- filename: jupyter-notebook-config-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Config API
  slug: jupyter-notebook-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-config-api-openapi.yml
- filename: jupyter-notebook-contents-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Contents API
  slug: jupyter-notebook-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-contents-api-openapi.yml
- filename: jupyter-notebook-general-api-openapi.yml
  format: yaml
  label: Jupyter Notebook General API
  slug: jupyter-notebook-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-general-api-openapi.yml
- filename: jupyter-notebook-groups-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Groups API
  slug: jupyter-notebook-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-groups-api-openapi.yml
- filename: jupyter-notebook-hub-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Hub API
  slug: jupyter-notebook-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-hub-api-openapi.yml
- filename: jupyter-notebook-kernels-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Kernels API
  slug: jupyter-notebook-kernels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-kernels-api-openapi.yml
- filename: jupyter-notebook-kernelspecs-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Kernelspecs API
  slug: jupyter-notebook-kernelspecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-kernelspecs-api-openapi.yml
- filename: jupyter-notebook-proxy-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Proxy API
  slug: jupyter-notebook-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-proxy-api-openapi.yml
- filename: jupyter-notebook-services-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Services API
  slug: jupyter-notebook-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-services-api-openapi.yml
- filename: jupyter-notebook-sessions-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Sessions API
  slug: jupyter-notebook-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-sessions-api-openapi.yml
- filename: jupyter-notebook-terminals-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Terminals API
  slug: jupyter-notebook-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-terminals-api-openapi.yml
- filename: jupyter-notebook-users-api-openapi.yml
  format: yaml
  label: Jupyter Notebook Users API
  slug: jupyter-notebook-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-users-api-openapi.yml
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
- Machine-Learning
- Notebooks
- Python
---
