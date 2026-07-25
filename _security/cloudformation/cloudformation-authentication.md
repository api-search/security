---
api_key_in:
- header
api_specs:
- filename: cloudformation-change-sets-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Change Sets API
  slug: cloudformation-change-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-change-sets-api-openapi.yml
- filename: cloudformation-exports-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Exports API
  slug: cloudformation-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-exports-api-openapi.yml
- filename: cloudformation-registry-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Registry API
  slug: cloudformation-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-registry-api-openapi.yml
- filename: cloudformation-request-status-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Request Status API
  slug: cloudformation-request-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-request-status-api-openapi.yml
- filename: cloudformation-resources-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Resources API
  slug: cloudformation-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-resources-api-openapi.yml
- filename: cloudformation-stack-drift-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Drift API
  slug: cloudformation-stack-drift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-drift-api-openapi.yml
- filename: cloudformation-stack-events-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Events API
  slug: cloudformation-stack-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-events-api-openapi.yml
- filename: cloudformation-stack-instances-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Instances API
  slug: cloudformation-stack-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-instances-api-openapi.yml
- filename: cloudformation-stack-policies-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Policies API
  slug: cloudformation-stack-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-policies-api-openapi.yml
- filename: cloudformation-stack-resources-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Resources API
  slug: cloudformation-stack-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-resources-api-openapi.yml
- filename: cloudformation-stack-sets-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Sets API
  slug: cloudformation-stack-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-sets-api-openapi.yml
- filename: cloudformation-stacks-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stacks API
  slug: cloudformation-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stacks-api-openapi.yml
- filename: cloudformation-templates-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Templates API
  slug: cloudformation-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudformation Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS CloudFormation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS CloudFormation
provider_slug: cloudformation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: AWS_Signature_V4
  parameter: Authorization
  sources:
  - openapi/cloud-control-api.yml
  - openapi/cloudformation-api.yml
  type: apiKey
slug: cloudformation-authentication
source_filename: cloudformation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-control-api.yml, openapi/cloudformation-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWS_Signature_V4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/cloud-control-api.yml\n  - openapi/cloudformation-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/authentication/cloudformation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
---
