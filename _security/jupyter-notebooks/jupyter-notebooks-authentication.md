---
api_key_in: []
api_specs:
- filename: jupyter-notebooks-openapi.yml
  format: yaml
  label: Jupyter Notebook Server REST API
  slug: notebook-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jupyter Notebooks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jupyter Notebooks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jupyter Notebooks
provider_slug: jupyter-notebooks
scheme_count: 1
schemes:
- bearerFormat: Jupyter-Token
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/jupyter-notebooks-openapi.yml
  type: http
slug: jupyter-notebooks-authentication
source_filename: jupyter-notebooks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyter-notebooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Jupyter-Token\n  sources:\n  - openapi/jupyter-notebooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/authentication/jupyter-notebooks-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Science
- Interactive Computing
- Jupyter
- Notebooks
- Python
---
