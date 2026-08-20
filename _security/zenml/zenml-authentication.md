---
api_key_in: []
api_specs:
- filename: zenml-artifacts-api-openapi.yml
  format: yaml
  label: ZenML Artifacts API
  slug: zenml-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-artifacts-api-openapi.yml
- filename: zenml-auth-api-openapi.yml
  format: yaml
  label: ZenML Auth API
  slug: zenml-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-auth-api-openapi.yml
- filename: zenml-deployments-api-openapi.yml
  format: yaml
  label: ZenML Deployments API
  slug: zenml-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-deployments-api-openapi.yml
- filename: zenml-models-api-openapi.yml
  format: yaml
  label: ZenML Models API
  slug: zenml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-models-api-openapi.yml
- filename: zenml-pipeline-runs-api-openapi.yml
  format: yaml
  label: ZenML Pipeline Runs API
  slug: zenml-pipeline-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-pipeline-runs-api-openapi.yml
- filename: zenml-pipelines-api-openapi.yml
  format: yaml
  label: ZenML Pipelines API
  slug: zenml-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-pipelines-api-openapi.yml
- filename: zenml-projects-api-openapi.yml
  format: yaml
  label: ZenML Projects API
  slug: zenml-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-projects-api-openapi.yml
- filename: zenml-schedules-api-openapi.yml
  format: yaml
  label: ZenML Schedules API
  slug: zenml-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-schedules-api-openapi.yml
- filename: zenml-secrets-api-openapi.yml
  format: yaml
  label: ZenML Secrets API
  slug: zenml-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-secrets-api-openapi.yml
- filename: zenml-service-connectors-api-openapi.yml
  format: yaml
  label: ZenML Service Connectors API
  slug: zenml-service-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-service-connectors-api-openapi.yml
- filename: zenml-stack-components-api-openapi.yml
  format: yaml
  label: ZenML Stack Components API
  slug: zenml-stack-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-stack-components-api-openapi.yml
- filename: zenml-stacks-api-openapi.yml
  format: yaml
  label: ZenML Stacks API
  slug: zenml-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-stacks-api-openapi.yml
- filename: zenml-users-api-openapi.yml
  format: yaml
  label: ZenML Users API
  slug: zenml-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/openapi/zenml-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zenml Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenML secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZenML
provider_slug: zenml
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zenml-openapi.yml
  type: http
slug: zenml-authentication
source_filename: zenml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zenml-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenml/refs/heads/main/authentication/zenml-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine-Learning
- MLOps
- LLMOps
- Pipelines
- Open-Source
- Python
---
