---
api_key_in:
- header
api_specs:
- filename: amazon-iam-access-analyzer-access-preview-analyzerarn-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Access Preview#analyzerArn API
  slug: amazon-iam-access-analyzer-access-preview-analyzerarn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-access-preview-analyzerarn-api-openapi.yml
- filename: amazon-iam-access-analyzer-access-preview-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Access Preview API
  slug: amazon-iam-access-analyzer-access-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-access-preview-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzed Resource#analyzerArn&resourceArn API
  slug: amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzed-resource-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzed Resource API
  slug: amazon-iam-access-analyzer-analyzed-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzed-resource-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzer-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzer API
  slug: amazon-iam-access-analyzer-analyzer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzer-api-openapi.yml
- filename: amazon-iam-access-analyzer-archive-rule-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Archive Rule API
  slug: amazon-iam-access-analyzer-archive-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-archive-rule-api-openapi.yml
- filename: amazon-iam-access-analyzer-finding-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Finding API
  slug: amazon-iam-access-analyzer-finding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-finding-api-openapi.yml
- filename: amazon-iam-access-analyzer-policy-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Policy API
  slug: amazon-iam-access-analyzer-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-policy-api-openapi.yml
- filename: amazon-iam-access-analyzer-resource-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Resource API
  slug: amazon-iam-access-analyzer-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-resource-api-openapi.yml
- filename: amazon-iam-access-analyzer-tags-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Tags API
  slug: amazon-iam-access-analyzer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iam Access Analyzer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IAM Access Analyzer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iam-access-analyzer-openapi-original.yml
  type: apiKey
slug: amazon-iam-access-analyzer-authentication
source_filename: amazon-iam-access-analyzer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iam-access-analyzer-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iam-access-analyzer-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/authentication/amazon-iam-access-analyzer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
---
