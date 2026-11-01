---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloudformation-resources-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Resources API
  slug: amazon-cloudformation-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-resources-api-openapi.yml
- filename: amazon-cloudformation-stacks-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Stacks API
  slug: amazon-cloudformation-stacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-stacks-api-openapi.yml
- filename: amazon-cloudformation-templates-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Templates API
  slug: amazon-cloudformation-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-templates-api-openapi.yml
- filename: amazon-cloudformation-changesets-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Changesets API
  slug: amazon-cloudformation-changesets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-changesets-api-openapi.yml
- filename: amazon-cloudformation-generated-template-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Generated Template API
  slug: amazon-cloudformation-generated-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-generated-template-api-openapi.yml
- filename: amazon-cloudformation-operations-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Operations API
  slug: amazon-cloudformation-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-operations-api-openapi.yml
- filename: amazon-cloudformation-resource-scan-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Resource Scan API
  slug: amazon-cloudformation-resource-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-resource-scan-api-openapi.yml
- filename: amazon-cloudformation-stack-instance-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Stack Instance API
  slug: amazon-cloudformation-stack-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-stack-instance-api-openapi.yml
- filename: amazon-cloudformation-stack-refactor-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Stack Refactor API
  slug: amazon-cloudformation-stack-refactor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-stack-refactor-api-openapi.yml
- filename: amazon-cloudformation-stack-set-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Stack Set API
  slug: amazon-cloudformation-stack-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-stack-set-api-openapi.yml
- filename: amazon-cloudformation-stack-set-operation-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Stack Set Operation API
  slug: amazon-cloudformation-stack-set-operation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-stack-set-operation-api-openapi.yml
- filename: amazon-cloudformation-type-api-openapi.yml
  format: yaml
  label: Amazon CloudFormation Cloudformation Type API
  slug: amazon-cloudformation-type-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudformation/openapi/amazon-cloudformation-type-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Cloudformation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudFormation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_auth
  parameter: Authorization
  sources:
  - openapi/amazon-cloudformation-openapi.yml
  type: apiKey
slug: amazon-cloudformation-authentication
source_filename: amazon-cloudformation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloudformation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-cloudformation-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloudformation/authentication/amazon-cloudformation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
---
