---
api_key_in:
- header
api_specs:
- filename: amazon-aurora-db-cluster-endpoints-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Endpoints API
  slug: amazon-aurora-db-cluster-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-endpoints-api-openapi.yml
- filename: amazon-aurora-db-cluster-parameter-groups-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Parameter Groups API
  slug: amazon-aurora-db-cluster-parameter-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-parameter-groups-api-openapi.yml
- filename: amazon-aurora-db-cluster-snapshots-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Snapshots API
  slug: amazon-aurora-db-cluster-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-snapshots-api-openapi.yml
- filename: amazon-aurora-db-clusters-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Clusters API
  slug: amazon-aurora-db-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-clusters-api-openapi.yml
- filename: amazon-aurora-db-instances-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Instances API
  slug: amazon-aurora-db-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-instances-api-openapi.yml
- filename: amazon-aurora-global-clusters-api-openapi.yml
  format: yaml
  label: Amazon Aurora Global Clusters API
  slug: amazon-aurora-global-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-global-clusters-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Aurora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Aurora secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Aurora
provider_slug: amazon-aurora
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-aurora-openapi.yml
  type: apiKey
slug: amazon-aurora-authentication
source_filename: amazon-aurora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-aurora-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-aurora-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/authentication/amazon-aurora-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Aurora
- MySQL
- PostgreSQL
- Relational Database
---
