---
api_key_in: []
api_specs:
- filename: databricks-clusters-api-openapi.yml
  format: yaml
  label: Databricks Clusters API
  slug: databricks-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-clusters-api-openapi.yml
- filename: databricks-jobs-api-openapi.yml
  format: yaml
  label: Databricks Jobs API
  slug: databricks-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-jobs-api-openapi.yml
- filename: databricks-workspace-api-openapi.yml
  format: yaml
  label: Databricks Workspace API
  slug: databricks-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Databricks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Databricks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Databricks
provider_slug: databricks
scheme_count: 1
schemes:
- bearerFormat: PAT
  description: Databricks personal access token (PAT) or OAuth M2M token. Pass the token in the Authorization header as 'Bearer <token>'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/databricks-openapi.yml
  type: http
slug: databricks-authentication
source_filename: databricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/databricks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  description: Databricks personal access token (PAT) or OAuth M2M token. Pass the token in\n    the Authorization header as 'Bearer <token>'.\n  sources:\n  - openapi/databricks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/authentication/databricks-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Analytics
- Apache Spark
- Big Data
- Cleanrooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine-Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
---
