---
api_key_in: []
api_specs:
- filename: pipeline.swagger.json
  format: json
  label: Kubeflow Pipelines REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubeflow/pipelines/master/backend/api/v2beta1/swagger/pipeline.swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kubeflow Pipelines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubeflow Pipelines secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kubeflow Pipelines
provider_slug: kubeflow-pipelines
scheme_count: 1
schemes:
- description: Bearer token issued by your Kubeflow distribution's identity provider. Some deployments use a session cookie instead.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kubeflow-pipelines-openapi.yml
  type: http
slug: kubeflow-pipelines-authentication
source_filename: kubeflow-pipelines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kubeflow-pipelines-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued by your Kubeflow distribution's identity provider. Some deployments\n    use a session cookie instead.\n  sources:\n  - openapi/kubeflow-pipelines-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/authentication/kubeflow-pipelines-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Science
- Kubernetes
- Machine Learning
- MLOps
- Orchestration
- Pipelines
- Workflows
---
