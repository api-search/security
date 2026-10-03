---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codedeploy-applications-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy Applications API
  slug: amazon-codedeploy-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-applications-api-openapi.yml
- filename: amazon-codedeploy-deployments-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy Deployments API
  slug: amazon-codedeploy-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-deployments-api-openapi.yml
- filename: amazon-codedeploy-aws-codedeploy-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy AWS CodeDeploy API
  slug: amazon-codedeploy-aws-codedeploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-aws-codedeploy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Codedeploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeDeploy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codedeploy-openapi-original.yaml
  type: apiKey
slug: amazon-codedeploy-authentication
source_filename: amazon-codedeploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codedeploy-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codedeploy-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/authentication/amazon-codedeploy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
- Developer Tools
---
