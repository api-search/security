---
api_key_in:
- header
api_specs:
- filename: amazon-rekognition-openapi.yml
  format: yaml
  label: Amazon Rekognition
  slug: amazon-rekognition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Rekognition Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Rekognition secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
scheme_count: 1
schemes:
- description: AWS Signature Version 4. Include the Authorization header with AWS4-HMAC-SHA256 signature.
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-rekognition-openapi.yml
  type: apiKey
slug: amazon-rekognition-authentication
source_filename: amazon-rekognition-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-rekognition-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. Include the Authorization header with AWS4-HMAC-SHA256\n    signature.\n  sources:\n  - openapi/amazon-rekognition-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/authentication/amazon-rekognition-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Celebrity Recognition
- Computer Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine Learning
- Object Detection
- Text Detection
- Video Analysis
---
