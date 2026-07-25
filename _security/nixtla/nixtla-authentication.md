---
api_key_in: []
api_specs:
- filename: nixtla-anomaly-detection-api-openapi.yml
  format: yaml
  label: Nixtla Anomaly Detection API
  slug: nixtla-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-anomaly-detection-api-openapi.yml
- filename: nixtla-cross-validation-api-openapi.yml
  format: yaml
  label: Nixtla Cross Validation API
  slug: nixtla-cross-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-cross-validation-api-openapi.yml
- filename: nixtla-excluded-api-openapi.yml
  format: yaml
  label: Nixtla excluded API
  slug: nixtla-excluded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-excluded-api-openapi.yml
- filename: nixtla-finetune-api-openapi.yml
  format: yaml
  label: Nixtla Finetune API
  slug: nixtla-finetune-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-finetune-api-openapi.yml
- filename: nixtla-finetuned-models-api-openapi.yml
  format: yaml
  label: Nixtla Finetuned Models API
  slug: nixtla-finetuned-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-finetuned-models-api-openapi.yml
- filename: nixtla-forecast-api-openapi.yml
  format: yaml
  label: Nixtla Forecast API
  slug: nixtla-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-forecast-api-openapi.yml
- filename: nixtla-online-anomaly-detection-api-openapi.yml
  format: yaml
  label: Nixtla Online Anomaly Detection API
  slug: nixtla-online-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-online-anomaly-detection-api-openapi.yml
- filename: nixtla-validate-api-key-api-openapi.yml
  format: yaml
  label: Nixtla Validate Api Key API
  slug: nixtla-validate-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-validate-api-key-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nixtla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nixtla secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nixtla
provider_slug: nixtla
scheme_count: 1
schemes:
- description: HTTPBearer
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/nixtla-openapi-original.json
  type: http
slug: nixtla-authentication
source_filename: nixtla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nixtla-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: HTTPBearer\n  sources:\n  - openapi/nixtla-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/authentication/nixtla-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Time Series
- Forecasting
- Anomaly Detection
- Machine Learning
- Artificial Intelligence
- Foundation Model
- Predictive Analytics
- Data Science
---
