---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-personalize-datasets-api-openapi.yml
  format: yaml
  label: Amazon Personalize Datasets API
  slug: amazon-personalize-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-datasets-api-openapi.yml
- filename: amazon-personalize-batch-inference-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Batch Inference Job API
  slug: amazon-personalize-batch-inference-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-batch-inference-job-api-openapi.yml
- filename: amazon-personalize-batch-segment-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Batch Segment Job API
  slug: amazon-personalize-batch-segment-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-batch-segment-job-api-openapi.yml
- filename: amazon-personalize-campaign-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Campaign API
  slug: amazon-personalize-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-campaign-api-openapi.yml
- filename: amazon-personalize-data-deletion-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Data Deletion Job API
  slug: amazon-personalize-data-deletion-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-data-deletion-job-api-openapi.yml
- filename: amazon-personalize-dataset-export-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Export Job API
  slug: amazon-personalize-dataset-export-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-export-job-api-openapi.yml
- filename: amazon-personalize-dataset-group-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Group API
  slug: amazon-personalize-dataset-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-group-api-openapi.yml
- filename: amazon-personalize-dataset-import-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Import Job API
  slug: amazon-personalize-dataset-import-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-import-job-api-openapi.yml
- filename: amazon-personalize-event-tracker-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Event Tracker API
  slug: amazon-personalize-event-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-event-tracker-api-openapi.yml
- filename: amazon-personalize-filter-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Filter API
  slug: amazon-personalize-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-filter-api-openapi.yml
- filename: amazon-personalize-metric-attribution-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Metric Attribution API
  slug: amazon-personalize-metric-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-metric-attribution-api-openapi.yml
- filename: amazon-personalize-operations-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Operations API
  slug: amazon-personalize-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-operations-api-openapi.yml
- filename: amazon-personalize-recommender-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Recommender API
  slug: amazon-personalize-recommender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-recommender-api-openapi.yml
- filename: amazon-personalize-schema-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Schema API
  slug: amazon-personalize-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-schema-api-openapi.yml
- filename: amazon-personalize-solution-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Solution API
  slug: amazon-personalize-solution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-solution-api-openapi.yml
- filename: amazon-personalize-solution-version-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Solution Version API
  slug: amazon-personalize-solution-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-solution-version-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Personalize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Personalize secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Personalize
provider_slug: amazon-personalize
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-personalize-openapi.yml
  type: apiKey
slug: amazon-personalize-authentication
source_filename: amazon-personalize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-personalize-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-personalize-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-personalize/authentication/amazon-personalize-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Customer Experience
- Machine Learning
- Personalization
- Recommendations
---
