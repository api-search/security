---
api_key_in: []
api_specs:
- filename: kubeflow-pipelines-experiments-api-openapi.yml
  format: yaml
  label: Kubeflow Pipelines Experiments API
  slug: kubeflow-pipelines-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/openapi/kubeflow-pipelines-experiments-api-openapi.yml
- filename: kubeflow-pipelines-health-api-openapi.yml
  format: yaml
  label: Kubeflow Pipelines Health API
  slug: kubeflow-pipelines-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/openapi/kubeflow-pipelines-health-api-openapi.yml
- filename: kubeflow-pipelines-pipelines-api-openapi.yml
  format: yaml
  label: Kubeflow Pipelines Pipelines API
  slug: kubeflow-pipelines-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/openapi/kubeflow-pipelines-pipelines-api-openapi.yml
- filename: kubeflow-pipelines-pipelineversions-api-openapi.yml
  format: yaml
  label: Kubeflow Pipelines PipelineVersions API
  slug: kubeflow-pipelines-pipelineversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/openapi/kubeflow-pipelines-pipelineversions-api-openapi.yml
- filename: kubeflow-pipelines-runs-api-openapi.yml
  format: yaml
  label: Kubeflow Pipelines Runs API
  slug: kubeflow-pipelines-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/openapi/kubeflow-pipelines-runs-api-openapi.yml
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
- Machine-Learning
- MLOps
- Orchestration
- Pipelines
- Workflows
---
