---
api_key_in:
- header
api_specs:
- filename: amazon-data-pipeline-pipeline-objects-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipeline Objects API
  slug: amazon-data-pipeline-pipeline-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipeline-objects-api-openapi.yml
- filename: amazon-data-pipeline-pipeline-runs-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipeline Runs API
  slug: amazon-data-pipeline-pipeline-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipeline-runs-api-openapi.yml
- filename: amazon-data-pipeline-pipelines-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipelines API
  slug: amazon-data-pipeline-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipelines-api-openapi.yml
- filename: amazon-data-pipeline-tags-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Tags API
  slug: amazon-data-pipeline-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Data Pipeline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Data Pipeline secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-data-pipeline-openapi.yml
  type: apiKey
slug: amazon-data-pipeline-authentication
source_filename: amazon-data-pipeline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-data-pipeline-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-data-pipeline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/authentication/amazon-data-pipeline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
---
