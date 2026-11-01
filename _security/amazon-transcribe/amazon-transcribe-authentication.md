---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-transcribe-transcription-jobs-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcription Jobs API
  slug: amazon-transcribe-transcription-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-transcription-jobs-api-openapi.yml
- filename: amazon-transcribe-vocabularies-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Vocabularies API
  slug: amazon-transcribe-vocabularies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-vocabularies-api-openapi.yml
- filename: amazon-transcribe-call-analytics-category-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Call Analytics Category API
  slug: amazon-transcribe-call-analytics-category-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-call-analytics-category-api-openapi.yml
- filename: amazon-transcribe-call-analytics-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Call Analytics Job API
  slug: amazon-transcribe-call-analytics-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-call-analytics-job-api-openapi.yml
- filename: amazon-transcribe-language-model-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Language Model API
  slug: amazon-transcribe-language-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-language-model-api-openapi.yml
- filename: amazon-transcribe-medical-scribe-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Scribe Job API
  slug: amazon-transcribe-medical-scribe-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-scribe-job-api-openapi.yml
- filename: amazon-transcribe-medical-transcription-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Transcription Job API
  slug: amazon-transcribe-medical-transcription-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-transcription-job-api-openapi.yml
- filename: amazon-transcribe-medical-vocabulary-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Vocabulary API
  slug: amazon-transcribe-medical-vocabulary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-vocabulary-api-openapi.yml
- filename: amazon-transcribe-operations-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Operations API
  slug: amazon-transcribe-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-operations-api-openapi.yml
- filename: amazon-transcribe-vocabulary-filter-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Vocabulary Filter API
  slug: amazon-transcribe-vocabulary-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-vocabulary-filter-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Transcribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Transcribe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-transcribe-openapi.yml
  type: apiKey
slug: amazon-transcribe-authentication
source_filename: amazon-transcribe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-transcribe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-transcribe-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-transcribe/authentication/amazon-transcribe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Audio Processing
- Machine Learning
- Speech Recognition
- Speech-to-Text
- Transcription
---
