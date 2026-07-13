---
api_key_in: []
api_specs:
- filename: pipeline.swagger.json
  format: json
  label: Kubeflow Pipelines API
  slug: pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubeflow/pipelines/master/backend/api/v2beta1/swagger/pipeline.swagger.json
- filename: rest_predict_v2.yaml
  format: yaml
  label: KServe Inference API
  slug: kserve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kserve/kserve/master/docs/predict-api/v2/rest_predict_v2.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kubeflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubeflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kubeflow
provider_slug: kubeflow
scheme_count: 1
schemes:
- description: Bearer token issued by your Kubeflow distribution's identity provider. Some deployments use a session cookie instead.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kubeflow-openapi.yml
  type: http
slug: kubeflow-authentication
source_filename: kubeflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kubeflow-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued by your Kubeflow distribution's identity provider. Some deployments\n    use a session cookie instead.\n  sources:\n  - openapi/kubeflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeflow/refs/heads/main/authentication/kubeflow-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Deep Learning
- Kubernetes
- Machine Learning
- MLOps
- Model Serving
- Model Training
- Open Source
---
