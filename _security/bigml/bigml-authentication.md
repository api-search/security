---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: BigML REST API
  slug: bigml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bigml Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigML secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BigML
provider_slug: bigml
scheme_count: 1
schemes:
- description: 'Authenticate with username and api_key as query parameters. Example: ?username=myuser&api_key=a1b2c3...'
  in: query
  name: ApiKeyAuth
  parameter: username
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: bigml-authentication
source_filename: bigml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: username\n  description: 'Authenticate with username and api_key as query parameters. Example: ?username=myuser&api_key=a1b2c3...'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/authentication/bigml-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Machine Learning
- Artificial Intelligence
- Predictions
- Datasets
- Models
- Clustering
- Anomaly Detection
- Time Series
- Deep Learning
---
