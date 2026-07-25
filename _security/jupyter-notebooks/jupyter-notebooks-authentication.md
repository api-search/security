---
api_key_in: []
api_specs:
- filename: jupyter-notebooks-contents-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Contents API
  slug: jupyter-notebooks-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-contents-api-openapi.yml
- filename: jupyter-notebooks-kernels-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Kernels API
  slug: jupyter-notebooks-kernels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-kernels-api-openapi.yml
- filename: jupyter-notebooks-kernelspecs-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks KernelSpecs API
  slug: jupyter-notebooks-kernelspecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-kernelspecs-api-openapi.yml
- filename: jupyter-notebooks-sessions-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Sessions API
  slug: jupyter-notebooks-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-sessions-api-openapi.yml
- filename: jupyter-notebooks-terminals-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Terminals API
  slug: jupyter-notebooks-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-terminals-api-openapi.yml
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
