---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Modelbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modelbit secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Modelbit
provider_slug: modelbit
scheme_count: 2
schemes:
- description: API key created in Modelbit Settings and passed in the Authorization header of REST inference requests to a deployment. Keys can be scoped to limit access to deployed models.
  in: header
  name: DeploymentApiKey
  parameter_name: Authorization
  source: https://doc.modelbit.com/deployments/calling-the-rest-api/using-api-keys/
  type: apiKey
- description: The modelbit Python package establishes an authenticated session via mb.login() (browser/token based) for training-job, dataset, model-registry and deployment operations from a notebook or CI environment.
  name: SdkLogin
  source: https://doc.modelbit.com/api-reference/login/
  type: session
slug: modelbit-authentication
source_filename: modelbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://doc.modelbit.com/deployments/calling-the-rest-api/\ndocs: https://doc.modelbit.com/deployments/calling-the-rest-api/using-api-keys/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    Modelbit deployments are called as REST inference endpoints. Access can be\n    restricted with API keys created in the Settings area of the Modelbit\n    workspace; the key is sent to the deployment in the HTTP Authorization\n    header. The Python SDK (modelbit) authenticates the developer session via an\n    interactive login flow (mb.login()) rather than a static key.\nschemes:\n  - name: DeploymentApiKey\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: >-\n      API key created in Modelbit Settings and passed in the Authorization\n      header of REST inference requests to a deployment. Keys can be scoped to\n      limit access to deployed models.\n    source: https://doc.modelbit.com/deployments/calling-the-rest-api/using-api-keys/\n\
  \  - name: SdkLogin\n    type: session\n    description: >-\n      The modelbit Python package establishes an authenticated session via\n      mb.login() (browser/token based) for training-job, dataset, model-registry\n      and deployment operations from a notebook or CI environment.\n    source: https://doc.modelbit.com/api-reference/login/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelbit/refs/heads/main/authentication/modelbit-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai
- Machine Learning
- MLOps
- Model Deployment
- Model Inference
- Data Science
- Model Registry
---
