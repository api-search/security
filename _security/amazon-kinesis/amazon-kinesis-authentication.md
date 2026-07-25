---
api_key_in:
- header
api_specs:
- filename: amazon-kinesis-account-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Account API
  slug: amazon-kinesis-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-account-api-openapi.yml
- filename: amazon-kinesis-consumers-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Consumers API
  slug: amazon-kinesis-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-consumers-api-openapi.yml
- filename: amazon-kinesis-encryption-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Encryption API
  slug: amazon-kinesis-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-encryption-api-openapi.yml
- filename: amazon-kinesis-monitoring-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Monitoring API
  slug: amazon-kinesis-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-monitoring-api-openapi.yml
- filename: amazon-kinesis-policies-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Policies API
  slug: amazon-kinesis-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-policies-api-openapi.yml
- filename: amazon-kinesis-records-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Records API
  slug: amazon-kinesis-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-records-api-openapi.yml
- filename: amazon-kinesis-shards-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Shards API
  slug: amazon-kinesis-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-shards-api-openapi.yml
- filename: amazon-kinesis-streams-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Streams API
  slug: amazon-kinesis-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-streams-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.AddTagsToStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.ListTagsForStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.RemoveTagsFromStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kinesis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Kinesis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Kinesis
provider_slug: amazon-kinesis
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed with the access key ID and secret access key of an IAM principal.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kinesis-data-streams-openapi.yml
  - openapi/amazon-kinesis-openapi.yml
  type: apiKey
slug: amazon-kinesis-authentication
source_filename: amazon-kinesis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kinesis-data-streams-openapi.yml, openapi/amazon-kinesis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Requests must be signed with the access\n    key ID and secret access key of an IAM principal.\n  sources:\n  - openapi/amazon-kinesis-data-streams-openapi.yml\n  - openapi/amazon-kinesis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/authentication/amazon-kinesis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Big Data
- Data Processing
- Real-Time
- Streaming
---
