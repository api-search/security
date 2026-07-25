---
api_key_in:
- query
api_specs:
- filename: bigml-anomaly-detection-api-openapi.yml
  format: yaml
  label: BigML Anomaly Detection API
  slug: bigml-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-anomaly-detection-api-openapi.yml
- filename: bigml-batch-operations-api-openapi.yml
  format: yaml
  label: BigML Batch Operations API
  slug: bigml-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-batch-operations-api-openapi.yml
- filename: bigml-clustering-api-openapi.yml
  format: yaml
  label: BigML Clustering API
  slug: bigml-clustering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-clustering-api-openapi.yml
- filename: bigml-data-connectors-api-openapi.yml
  format: yaml
  label: BigML Data Connectors API
  slug: bigml-data-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-data-connectors-api-openapi.yml
- filename: bigml-datasets-api-openapi.yml
  format: yaml
  label: BigML Datasets API
  slug: bigml-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-datasets-api-openapi.yml
- filename: bigml-ensembles-api-openapi.yml
  format: yaml
  label: BigML Ensembles API
  slug: bigml-ensembles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-ensembles-api-openapi.yml
- filename: bigml-evaluations-api-openapi.yml
  format: yaml
  label: BigML Evaluations API
  slug: bigml-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-evaluations-api-openapi.yml
- filename: bigml-models-api-openapi.yml
  format: yaml
  label: BigML Models API
  slug: bigml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-models-api-openapi.yml
- filename: bigml-predictions-api-openapi.yml
  format: yaml
  label: BigML Predictions API
  slug: bigml-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-predictions-api-openapi.yml
- filename: bigml-projects-api-openapi.yml
  format: yaml
  label: BigML Projects API
  slug: bigml-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-projects-api-openapi.yml
- filename: bigml-sources-api-openapi.yml
  format: yaml
  label: BigML Sources API
  slug: bigml-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-sources-api-openapi.yml
- filename: bigml-supervised-learning-api-openapi.yml
  format: yaml
  label: BigML Supervised Learning API
  slug: bigml-supervised-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-supervised-learning-api-openapi.yml
- filename: bigml-time-series-api-openapi.yml
  format: yaml
  label: BigML Time Series API
  slug: bigml-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-time-series-api-openapi.yml
- filename: bigml-unsupervised-learning-api-openapi.yml
  format: yaml
  label: BigML Unsupervised Learning API
  slug: bigml-unsupervised-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-unsupervised-learning-api-openapi.yml
- filename: bigml-whizzml-scripting-api-openapi.yml
  format: yaml
  label: BigML WhizzML Scripting API
  slug: bigml-whizzml-scripting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-whizzml-scripting-api-openapi.yml
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
