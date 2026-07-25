---
api_key_in:
- header
api_specs:
- filename: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
  format: yaml
  label: Amazon ECR Amazon ECR Amazon Elastic Container Registry (ECR) API API
  slug: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
- filename: amazon-ecr-batchgetimage-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #BatchGetImage API'
  slug: amazon-ecr-batchgetimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-batchgetimage-api-openapi.yml
- filename: amazon-ecr-deleterepository-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #DeleteRepository API'
  slug: amazon-ecr-deleterepository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-deleterepository-api-openapi.yml
- filename: amazon-ecr-describerepositories-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #DescribeRepositories API'
  slug: amazon-ecr-describerepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-describerepositories-api-openapi.yml
- filename: amazon-ecr-listimages-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #ListImages API'
  slug: amazon-ecr-listimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-listimages-api-openapi.yml
- filename: amazon-ecr-putimage-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #PutImage API'
  slug: amazon-ecr-putimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-putimage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ecr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon ECR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon ECR
provider_slug: amazon-ecr
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-ecr-openapi.yml
  type: apiKey
slug: amazon-ecr-authentication
source_filename: amazon-ecr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ecr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-ecr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/authentication/amazon-ecr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
---
