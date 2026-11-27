---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kinesis-liststreams-api-openapi.yml
  format: yaml
  label: AWS Kinesis ListStreams API
  slug: kinesis-liststreams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-liststreams-api-openapi.yml
- filename: kinesis-amazon-kinesis-analytics-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis Analytics API
  slug: kinesis-amazon-kinesis-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-analytics-api-openapi.yml
- filename: kinesis-amazon-kinesis-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis API
  slug: kinesis-amazon-kinesis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-api-openapi.yml
- filename: kinesis-amazon-kinesis-firehose-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis Firehose API
  slug: kinesis-amazon-kinesis-firehose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-firehose-api-openapi.yml
- filename: kinesis-channel-api-openapi.yml
  format: yaml
  label: AWS Kinesis Channel API
  slug: kinesis-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-channel-api-openapi.yml
- filename: kinesis-operations-api-openapi.yml
  format: yaml
  label: AWS Kinesis Operations API
  slug: kinesis-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-operations-api-openapi.yml
- filename: kinesis-resource-policy-api-openapi.yml
  format: yaml
  label: AWS Kinesis Resource Policy API
  slug: kinesis-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-resource-policy-api-openapi.yml
- filename: kinesis-create-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Create Stream API
  slug: kinesis-create-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-create-stream-api-openapi.yml
- filename: kinesis-delete-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Delete Stream API
  slug: kinesis-delete-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-delete-stream-api-openapi.yml
- filename: kinesis-describe-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Describe Stream API
  slug: kinesis-describe-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-describe-stream-api-openapi.yml
- filename: kinesis-list-tags-for-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis List Tags For Resource API
  slug: kinesis-list-tags-for-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-list-tags-for-resource-api-openapi.yml
- filename: kinesis-list-tags-for-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis List Tags For Stream API
  slug: kinesis-list-tags-for-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-list-tags-for-stream-api-openapi.yml
- filename: kinesis-tag-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis Tag Resource API
  slug: kinesis-tag-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-tag-resource-api-openapi.yml
- filename: kinesis-untag-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis Untag Resource API
  slug: kinesis-untag-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-untag-resource-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AWS Kinesis Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Kinesis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Kinesis
provider_slug: kinesis
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/kinesis-amazon-kinesis-analytics-api-openapi.yml
  - openapi/kinesis-amazon-kinesis-api-openapi.yml
  - openapi/kinesis-amazon-kinesis-firehose-api-openapi.yml
  - openapi/kinesis-channel-api-openapi.yml
  - openapi/kinesis-create-stream-api-openapi.yml
  - openapi/kinesis-delete-stream-api-openapi.yml
  - openapi/kinesis-describe-stream-api-openapi.yml
  - openapi/kinesis-list-tags-for-resource-api-openapi.yml
  - openapi/kinesis-list-tags-for-stream-api-openapi.yml
  - openapi/kinesis-liststreams-api-openapi.yml
  - openapi/kinesis-operations-api-openapi.yml
  - openapi/kinesis-resource-policy-api-openapi.yml
  - openapi/kinesis-tag-resource-api-openapi.yml
  - openapi/kinesis-untag-resource-api-openapi.yml
  type: apiKey
slug: kinesis-authentication
source_filename: kinesis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/kinesis-amazon-kinesis-analytics-api-openapi.yml, openapi/kinesis-amazon-kinesis-api-openapi.yml,\n  openapi/kinesis-amazon-kinesis-firehose-api-openapi.yml, openapi/kinesis-channel-api-openapi.yml,\n  openapi/kinesis-create-stream-api-openapi.yml, openapi/kinesis-delete-stream-api-openapi.yml,\n  openapi/kinesis-describe-stream-api-openapi.yml, openapi/kinesis-list-tags-for-resource-api-openapi.yml,\n  openapi/kinesis-list-tags-for-stream-api-openapi.yml, openapi/kinesis-liststreams-api-openapi.yml,\n  openapi/kinesis-operations-api-openapi.yml, openapi/kinesis-resource-policy-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for\
  \ temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/kinesis-amazon-kinesis-analytics-api-openapi.yml\n  - openapi/kinesis-amazon-kinesis-api-openapi.yml\n  - openapi/kinesis-amazon-kinesis-firehose-api-openapi.yml\n  - openapi/kinesis-channel-api-openapi.yml\n  - openapi/kinesis-create-stream-api-openapi.yml\n  - openapi/kinesis-delete-stream-api-openapi.yml\n  - openapi/kinesis-describe-stream-api-openapi.yml\n  - openapi/kinesis-list-tags-for-resource-api-openapi.yml\n  - openapi/kinesis-list-tags-for-stream-api-openapi.yml\n  - openapi/kinesis-liststreams-api-openapi.yml\n  - openapi/kinesis-operations-api-openapi.yml\n  - openapi/kinesis-resource-policy-api-openapi.yml\n  - openapi/kinesis-tag-resource-api-openapi.yml\n  - openapi/kinesis-untag-resource-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/kinesis/authentication/kinesis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Apache Flink
- Amazon Web Services
- Big Data
- Data Processing
- Real-Time
- Streaming
- Video
---
