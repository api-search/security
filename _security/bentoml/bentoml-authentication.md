---
api_key_in:
- header
api_specs:
- filename: bentoml-bentocloud-deployment-api-openapi.yml
  format: yaml
  label: BentoCloud Deployment API
  slug: bentocloud-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bentoml/refs/heads/main/openapi/bentoml-bentocloud-deployment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bentoml Authentication
name_suffix: Authentication
oauth_flows: []
overview: BentoML secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BentoML
provider_slug: bentoml
scheme_count: 1
schemes:
- in: header
  name: apiToken
  parameter: X-YATAI-API-TOKEN
  sources:
  - openapi/bentoml-bentocloud-deployment-api-openapi.yml
  type: apiKey
slug: bentoml-authentication
source_filename: bentoml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bentoml-bentocloud-deployment-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: X-YATAI-API-TOKEN\n  sources:\n  - openapi/bentoml-bentocloud-deployment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bentoml/refs/heads/main/authentication/bentoml-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- machine learning
- model serving
- inference
- AI
- REST API
- MLOps
- deployment
- GPU
- LLM
- BentoCloud
---
