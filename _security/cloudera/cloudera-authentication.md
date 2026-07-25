---
api_key_in:
- header
api_specs:
- filename: cloudera-dataengineering-api-openapi.yml
  format: yaml
  label: Cloudera DataEngineering API
  slug: cloudera-dataengineering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-dataengineering-api-openapi.yml
- filename: cloudera-datahub-api-openapi.yml
  format: yaml
  label: Cloudera Datahub API
  slug: cloudera-datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datahub-api-openapi.yml
- filename: cloudera-datalake-api-openapi.yml
  format: yaml
  label: Cloudera Datalake API
  slug: cloudera-datalake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datalake-api-openapi.yml
- filename: cloudera-environments-api-openapi.yml
  format: yaml
  label: Cloudera Environments API
  slug: cloudera-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-environments-api-openapi.yml
- filename: cloudera-iam-api-openapi.yml
  format: yaml
  label: Cloudera IAM API
  slug: cloudera-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-iam-api-openapi.yml
- filename: cloudera-ml-api-openapi.yml
  format: yaml
  label: Cloudera ML API
  slug: cloudera-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-ml-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudera secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudera
provider_slug: cloudera
scheme_count: 1
schemes:
- description: 'CDP signature-based authentication. Each request must include an

    x-altus-auth signature header and an x-altus-date timestamp header.'
  in: header
  name: altusAuth
  parameter: x-altus-auth
  sources:
  - openapi/cloudera-openapi.yml
  type: apiKey
slug: cloudera-authentication
source_filename: cloudera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudera-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: altusAuth\n  type: apiKey\n  in: header\n  parameter: x-altus-auth\n  description: |-\n    CDP signature-based authentication. Each request must include an\n    x-altus-auth signature header and an x-altus-date timestamp header.\n  sources:\n  - openapi/cloudera-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/authentication/cloudera-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Big Data
- Data Engineering
- Data Lakehouse
- Data Platform
- Data Warehouse
- Hadoop
- Hybrid Cloud
- Machine Learning
- Streaming
---
