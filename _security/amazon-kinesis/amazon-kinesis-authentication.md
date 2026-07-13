---
api_key_in:
- header
api_specs:
- filename: amazon-kinesis-data-streams-openapi.yml
  format: yaml
  label: Amazon Kinesis Data Streams
  slug: amazon-kinesis-data-streams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-data-streams-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Amazon Data Firehose
  slug: amazon-data-firehose
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/firehose/2015-08-04/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Managed Service for Apache Flink
  slug: amazon-managed-service-for-apache-flink
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisanalyticsv2/2018-05-23/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams
  slug: amazon-kinesis-video-streams
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisvideo/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams Media
  slug: amazon-kinesis-video-streams-media
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-media/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams Archived Media
  slug: amazon-kinesis-video-streams-archived-media
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-archived-media/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Signaling Channels
  slug: amazon-kinesis-video-signaling-channels
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-signaling/2019-12-04/openapi.yaml
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
