---
api_key_in: []
api_specs:
- filename: amazon-sns-api-openapi.yml
  format: yaml
  label: Amazon SNS API
  slug: amazon-sns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Sns Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SNS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SNS
provider_slug: amazon-sns
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials with appropriate SNS permissions. See https://docs.aws.amazon.com/general/latest/gr/signing_aws_api_requests.html
  name: AWS_IAM
  scheme: bearer
  sources:
  - openapi/amazon-sns-api-openapi.yml
  type: http
slug: amazon-sns-authentication
source_filename: amazon-sns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-sns-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: AWS_IAM\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials\n    with appropriate SNS permissions. See https://docs.aws.amazon.com/general/latest/gr/signing_aws_api_requests.html\n  sources:\n  - openapi/amazon-sns-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/authentication/amazon-sns-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
---
