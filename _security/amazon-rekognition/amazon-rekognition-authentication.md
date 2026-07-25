---
api_key_in:
- header
api_specs:
- filename: amazon-rekognition-celebrity-recognition-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Celebrity Recognition API
  slug: amazon-rekognition-celebrity-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-celebrity-recognition-api-openapi.yml
- filename: amazon-rekognition-content-moderation-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Content Moderation API
  slug: amazon-rekognition-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-content-moderation-api-openapi.yml
- filename: amazon-rekognition-custom-labels-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Custom Labels API
  slug: amazon-rekognition-custom-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-custom-labels-api-openapi.yml
- filename: amazon-rekognition-face-collections-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Collections API
  slug: amazon-rekognition-face-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-collections-api-openapi.yml
- filename: amazon-rekognition-face-liveness-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Liveness API
  slug: amazon-rekognition-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-liveness-api-openapi.yml
- filename: amazon-rekognition-face-search-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Search API
  slug: amazon-rekognition-face-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-search-api-openapi.yml
- filename: amazon-rekognition-facial-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Facial Analysis API
  slug: amazon-rekognition-facial-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-facial-analysis-api-openapi.yml
- filename: amazon-rekognition-image-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Image Analysis API
  slug: amazon-rekognition-image-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-image-analysis-api-openapi.yml
- filename: amazon-rekognition-stored-video-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Stored Video Analysis API
  slug: amazon-rekognition-stored-video-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-stored-video-analysis-api-openapi.yml
- filename: amazon-rekognition-text-detection-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Text Detection API
  slug: amazon-rekognition-text-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-text-detection-api-openapi.yml
auth_types:
- apiKey
description: Amazon Rekognition authorizes requests with AWS Identity and Access Management (IAM). Every call must be signed with AWS Signature Version 4 (SigV4) using the caller's access key / temporary credentials; the OpenAPI models this as an apiKey scheme on the Authorization header. Fine-grained authorization is controlled by IAM policies (e.g. AmazonRekognitionFullAccess, AmazonRekognitionReadOnlyAccess) and rekognition:* actions.
kind: authentication
layout: security
method: searched
name: Amazon Rekognition Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Rekognition secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
scheme_count: 1
schemes:
- description: AWS Signature Version 4. Include the Authorization header with AWS4-HMAC-SHA256 signature computed from AWS IAM credentials.
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
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/amazon-rekognition-openapi.yml\ndocs: https://docs.aws.amazon.com/rekognition/latest/dg/security_iam_service-with-iam.html\ndescription: >-\n  Amazon Rekognition authorizes requests with AWS Identity and Access Management\n  (IAM). Every call must be signed with AWS Signature Version 4 (SigV4) using the\n  caller's access key / temporary credentials; the OpenAPI models this as an\n  apiKey scheme on the Authorization header. Fine-grained authorization is\n  controlled by IAM policies (e.g. AmazonRekognitionFullAccess,\n  AmazonRekognitionReadOnlyAccess) and rekognition:* actions.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  authorization: AWS IAM (SigV4)\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. Include the Authorization header with AWS4-HMAC-SHA256\n    signature computed from AWS IAM credentials.\n  sources:\n\
  \  - openapi/amazon-rekognition-openapi.yml\niam:\n  managed_policies:\n    - AmazonRekognitionFullAccess\n    - AmazonRekognitionReadOnlyAccess\n    - AmazonRekognitionCustomLabelsFullAccess\n  action_prefix: \"rekognition:\"\n  docs: https://docs.aws.amazon.com/rekognition/latest/dg/security-iam-awsmanpol.html\n"
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
