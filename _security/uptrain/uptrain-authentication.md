---
api_key_in:
- header
api_specs:
- filename: uptrain-auth-api-openapi.yml
  format: yaml
  label: UpTrain Auth API
  slug: uptrain-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-auth-api-openapi.yml
- filename: uptrain-checksets-api-openapi.yml
  format: yaml
  label: UpTrain Checksets API
  slug: uptrain-checksets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-checksets-api-openapi.yml
- filename: uptrain-datasets-api-openapi.yml
  format: yaml
  label: UpTrain Datasets API
  slug: uptrain-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-datasets-api-openapi.yml
- filename: uptrain-evaluation-api-openapi.yml
  format: yaml
  label: UpTrain Evaluation API
  slug: uptrain-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-evaluation-api-openapi.yml
- filename: uptrain-root-cause-analysis-api-openapi.yml
  format: yaml
  label: UpTrain Root Cause Analysis API
  slug: uptrain-root-cause-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-root-cause-analysis-api-openapi.yml
- filename: uptrain-runs-api-openapi.yml
  format: yaml
  label: UpTrain Runs API
  slug: uptrain-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-runs-api-openapi.yml
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
- Artificial Intelligence
- LLM
- Evaluation
- LLM Evaluation
- Observability
- Open-Source
---
