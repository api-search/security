---
api_key_in:
- header
api_specs:
- filename: amazon-deepracer-openapi.yml
  format: yaml
  label: AWS DeepRacer API
  slug: aws-deepracer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/openapi/amazon-deepracer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Deepracer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DeepRacer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Sign requests using your AWS access key, secret key, and session token.
  in: header
  name: awsSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-deepracer-openapi.yml
  type: apiKey
slug: amazon-deepracer-authentication
source_filename: amazon-deepracer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-deepracer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Sign requests using your AWS access key,\n    secret key, and session token.\n  sources:\n  - openapi/amazon-deepracer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/authentication/amazon-deepracer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
---
