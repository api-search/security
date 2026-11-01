---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-lookout-for-equipment-datasets-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Datasets API
  slug: amazon-lookout-for-equipment-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-datasets-api-openapi.yml
- filename: amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Data Ingestion Job API
  slug: amazon-lookout-for-equipment-data-ingestion-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
- filename: amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Inference Scheduler API
  slug: amazon-lookout-for-equipment-inference-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label API
  slug: amazon-lookout-for-equipment-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-group-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label Group API
  slug: amazon-lookout-for-equipment-label-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-group-api-openapi.yml
- filename: amazon-lookout-for-equipment-model-version-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Model Version API
  slug: amazon-lookout-for-equipment-model-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-model-version-api-openapi.yml
- filename: amazon-lookout-for-equipment-operations-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Operations API
  slug: amazon-lookout-for-equipment-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-operations-api-openapi.yml
- filename: amazon-lookout-for-equipment-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Resource Policy API
  slug: amazon-lookout-for-equipment-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-resource-policy-api-openapi.yml
- filename: amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Retraining Scheduler API
  slug: amazon-lookout-for-equipment-retraining-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Lookout For Equipment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lookout for Equipment secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-lookout-for-equipment-openapi.yml
  type: apiKey
slug: amazon-lookout-for-equipment-authentication
source_filename: amazon-lookout-for-equipment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-lookout-for-equipment-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-lookout-for-equipment-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-lookout-for-equipment/authentication/amazon-lookout-for-equipment-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
---
