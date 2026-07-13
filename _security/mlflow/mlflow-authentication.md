---
api_key_in: []
api_specs:
- filename: mlflow-openapi.yml
  format: yaml
  label: MLflow REST API
  slug: mlflow-tracking-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mlflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: MLflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MLflow
provider_slug: mlflow
scheme_count: 1
schemes:
- description: 'Optional HTTP Basic authentication when the MLflow tracking server is

    configured with the `mlflow-basic-auth` plugin. Default open-source

    servers run without authentication.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mlflow-openapi.yml
  type: http
slug: mlflow-authentication
source_filename: mlflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mlflow-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Optional HTTP Basic authentication when the MLflow tracking server is\n    configured with the `mlflow-basic-auth` plugin. Default open-source\n    servers run without authentication.\n  sources:\n  - openapi/mlflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/authentication/mlflow-authentication.yml
summary_line: http · 1 scheme
tags:
- ML
- MLOps
- GenAI
- Experiment Tracking
- Open Source
---
