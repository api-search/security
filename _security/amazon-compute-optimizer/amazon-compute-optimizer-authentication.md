---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-compute-optimizer-aws-compute-optimizer-api-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer AWS Compute Optimizer API
  slug: amazon-compute-optimizer-aws-compute-optimizer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-compute-optimizer/openapi/amazon-compute-optimizer-aws-compute-optimizer-api-openapi.yml
- filename: amazon-compute-optimizer-operations-api-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer Compute Optimizer Operations API
  slug: amazon-compute-optimizer-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-compute-optimizer/openapi/amazon-compute-optimizer-operations-api-openapi.yml
- filename: amazon-compute-optimizer-account-api-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer Compute Optimizer Account API
  slug: amazon-compute-optimizer-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-compute-optimizer/openapi/amazon-compute-optimizer-account-api-openapi.yml
- filename: amazon-compute-optimizer-automation-event-api-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer Compute Optimizer Automation Event API
  slug: amazon-compute-optimizer-automation-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-compute-optimizer/openapi/amazon-compute-optimizer-automation-event-api-openapi.yml
- filename: amazon-compute-optimizer-automation-rule-api-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer Compute Optimizer Automation Rule API
  slug: amazon-compute-optimizer-automation-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-compute-optimizer/openapi/amazon-compute-optimizer-automation-rule-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Compute Optimizer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Compute Optimizer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-compute-optimizer-account-api-openapi.yml
  - openapi/amazon-compute-optimizer-automation-event-api-openapi.yml
  - openapi/amazon-compute-optimizer-automation-rule-api-openapi.yml
  - openapi/amazon-compute-optimizer-aws-compute-optimizer-api-openapi.yml
  - openapi/amazon-compute-optimizer-operations-api-openapi.yml
  type: apiKey
slug: amazon-compute-optimizer-authentication
source_filename: amazon-compute-optimizer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-compute-optimizer-account-api-openapi.yml, openapi/amazon-compute-optimizer-automation-event-api-openapi.yml,\n  openapi/amazon-compute-optimizer-automation-rule-api-openapi.yml, openapi/amazon-compute-optimizer-aws-compute-optimizer-api-openapi.yml,\n  openapi/amazon-compute-optimizer-operations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-compute-optimizer-account-api-openapi.yml\n  - openapi/amazon-compute-optimizer-automation-event-api-openapi.yml\n  - openapi/amazon-compute-optimizer-automation-rule-api-openapi.yml\n  - openapi/amazon-compute-optimizer-aws-compute-optimizer-api-openapi.yml\n\
  \  - openapi/amazon-compute-optimizer-operations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-compute-optimizer/authentication/amazon-compute-optimizer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
---
