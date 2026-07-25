---
api_key_in: []
api_specs:
- filename: jupyter-hub-groups-api-openapi.yml
  format: yaml
  label: JupyterHub Groups API
  slug: jupyter-hub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-groups-api-openapi.yml
- filename: jupyter-hub-hub-api-openapi.yml
  format: yaml
  label: JupyterHub Hub API
  slug: jupyter-hub-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-hub-api-openapi.yml
- filename: jupyter-hub-services-api-openapi.yml
  format: yaml
  label: JupyterHub Services API
  slug: jupyter-hub-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-services-api-openapi.yml
- filename: jupyter-hub-tokens-api-openapi.yml
  format: yaml
  label: JupyterHub Tokens API
  slug: jupyter-hub-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-tokens-api-openapi.yml
- filename: jupyter-hub-users-api-openapi.yml
  format: yaml
  label: JupyterHub Users API
  slug: jupyter-hub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jupyter Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: JupyterHub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JupyterHub
provider_slug: jupyter-hub
scheme_count: 1
schemes:
- bearerFormat: JupyterHub-Token
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/jupyter-hub-openapi.yml
  type: http
slug: jupyter-hub-authentication
source_filename: jupyter-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyter-hub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JupyterHub-Token\n  sources:\n  - openapi/jupyter-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/authentication/jupyter-hub-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Science
- Education
- Jupyter
- Multi-User
- Notebooks
---
