---
api_key_in:
- query
api_specs:
- filename: truth-systems-gateway-openapi-original.json
  format: json
  label: Truth Systems Gateway API
  slug: truth-systems-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truth-systems/refs/heads/main/openapi/truth-systems-gateway-openapi-original.json
auth_types:
- aws-iam
- apiKey
description: Authentication profile for the Truth Systems Gateway API. Gateway deploys into the customer's own cloud account (AWS or Azure), so authentication is cloud-native rather than a hosted API key or OAuth surface. The published OpenAPI declares no securitySchemes (the HTTP surface is reached inside the customer deployment); auth is documented on the SDK usage page.
kind: authentication
layout: security
method: searched
name: Truth Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truth Systems secures its APIs with aws-iam and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Truth Systems
provider_slug: truth-systems
scheme_count: 2
schemes:
- description: On AWS, the AwsClient invokes the Gateway Step Function with the caller's AWS credentials (environment variables, IAM role, or ~/.aws/credentials). Callers need IAM permissions states:StartExecution and states:DescribeExecution on the deployed state machine.
  docs: https://docs.truthsystems.ai/sdk/usage
  name: aws-iam
  type: aws-iam
- description: On Azure, the AzureClient authenticates with the Function App's function key passed at construction time (available as the Terraform output function_app_default_key). No Azure AD roles are required - anyone with the key can invoke Gateway.
  docs: https://docs.truthsystems.ai/deployment/azure
  in: query
  name: azure-function-key
  type: apiKey
slug: truth-systems-authentication
source_filename: truth-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.truthsystems.ai/sdk/usage\ndescription: >-\n  Authentication profile for the Truth Systems Gateway API. Gateway deploys\n  into the customer's own cloud account (AWS or Azure), so authentication is\n  cloud-native rather than a hosted API key or OAuth surface. The published\n  OpenAPI declares no securitySchemes (the HTTP surface is reached inside the\n  customer deployment); auth is documented on the SDK usage page.\nsummary:\n  types: [aws-iam, apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: aws-iam\n    type: aws-iam\n    description: >-\n      On AWS, the AwsClient invokes the Gateway Step Function with the caller's\n      AWS credentials (environment variables, IAM role, or ~/.aws/credentials).\n      Callers need IAM permissions states:StartExecution and\n      states:DescribeExecution on the deployed state machine.\n    docs: https://docs.truthsystems.ai/sdk/usage\n  - name: azure-function-key\n\
  \    type: apiKey\n    in: query\n    description: >-\n      On Azure, the AzureClient authenticates with the Function App's function\n      key passed at construction time (available as the Terraform output\n      function_app_default_key). No Azure AD roles are required - anyone with\n      the key can invoke Gateway.\n    docs: https://docs.truthsystems.ai/deployment/azure\nnotes:\n  - The OpenAPI (openapi/truth-systems-gateway-openapi-original.json) defines\n    no securitySchemes; this profile is taken from the published docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truth-systems/refs/heads/main/authentication/truth-systems-authentication.yml
summary_line: aws-iam/apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Governance
- Hallucination Detection
- Fact Checking
- Compliance
- Legal
---
