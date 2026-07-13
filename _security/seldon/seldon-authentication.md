---
api_key_in: []
api_specs:
- filename: engine.oas3.json
  format: json
  label: Seldon Inference API
  slug: seldon-inference-api
  spec_type: OpenAPI
  url: https://github.com/SeldonIO/seldon-core/blob/master/openapi/engine.oas3.json
- filename: seldon-enterprise-platform-api-openapi.yml
  format: yaml
  label: Seldon Enterprise Platform REST API
  slug: seldon-enterprise-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/openapi/seldon-enterprise-platform-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Seldon Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Seldon secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Seldon
provider_slug: seldon
scheme_count: 2
schemes:
- flows:
  - flow: password
    scopes: 4
    tokenUrl: https://Y.Y.Y.Y
  name: OAuth2
  sources:
  - openapi/seldon-enterprise-platform-api-openapi.yml
  type: oauth2
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/seldon-inference-api-openapi.yml
  type: http
slug: seldon-authentication
source_filename: seldon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seldon-enterprise-platform-api-openapi.yml, openapi/seldon-inference-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://Y.Y.Y.Y\n    scopes: 4\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/seldon-inference-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/authentication/seldon-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- MLOps
- Machine Learning
- Model Serving
- Inference
- Kubernetes
- AI Operations
- Drift Detection
- Explainability
- Canary Deployment
- A/B Testing
- LLMOps
---
