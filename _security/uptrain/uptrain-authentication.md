---
api_key_in:
- header
api_specs:
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Evaluations API
  slug: uptrain-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Log and Evaluate API
  slug: uptrain-log-and-evaluate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Root Cause Analysis API
  slug: uptrain-root-cause-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Runs and Datasets API
  slug: uptrain-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uptrain Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpTrain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpTrain
provider_slug: uptrain
scheme_count: 1
schemes:
- description: UpTrain managed-service access token. Obtained from the UpTrain dashboard and supplied on every request as the uptrain-access-token header.
  in: header
  name: UptrainAccessToken
  parameter: uptrain-access-token
  sources:
  - openapi/uptrain-openapi.yml
  type: apiKey
slug: uptrain-authentication
source_filename: uptrain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uptrain-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: UptrainAccessToken\n  type: apiKey\n  in: header\n  parameter: uptrain-access-token\n  description: UpTrain managed-service access token. Obtained from the UpTrain dashboard and\n    supplied on every request as the uptrain-access-token header.\n  sources:\n  - openapi/uptrain-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/authentication/uptrain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Evaluation
- LLM Evaluation
- Observability
- Open Source
---
