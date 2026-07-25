---
api_key_in:
- query
api_specs:
- filename: google-cloud-dataflow-debug-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Debug API
  slug: google-cloud-dataflow-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-debug-api-openapi.yml
- filename: google-cloud-dataflow-flex-templates-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Flex Templates API
  slug: google-cloud-dataflow-flex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-flex-templates-api-openapi.yml
- filename: google-cloud-dataflow-jobs-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Jobs API
  slug: google-cloud-dataflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-jobs-api-openapi.yml
- filename: google-cloud-dataflow-messages-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Messages API
  slug: google-cloud-dataflow-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-messages-api-openapi.yml
- filename: google-cloud-dataflow-metrics-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Metrics API
  slug: google-cloud-dataflow-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-metrics-api-openapi.yml
- filename: google-cloud-dataflow-snapshots-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Snapshots API
  slug: google-cloud-dataflow-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-snapshots-api-openapi.yml
- filename: google-cloud-dataflow-stages-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Stages API
  slug: google-cloud-dataflow-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-stages-api-openapi.yml
- filename: google-cloud-dataflow-templates-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Templates API
  slug: google-cloud-dataflow-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-templates-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Dataflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Dataflow secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for Google Cloud APIs.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-cloud-dataflow-api-openapi.yml
  type: oauth2
- description: API key for identifying the calling project.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-cloud-dataflow-api-openapi.yml
  type: apiKey
slug: google-cloud-dataflow-authentication
source_filename: google-cloud-dataflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-dataflow-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  description: OAuth 2.0 authentication for Google Cloud APIs.\n  sources:\n  - openapi/google-cloud-dataflow-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key for identifying the calling project.\n  sources:\n  - openapi/google-cloud-dataflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/authentication/google-cloud-dataflow-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
---
