---
anonymous_access: false
api_key_in: []
api_specs:
- filename: auxen-ai-billing-api-openapi.yml
  format: yaml
  label: Auxen Billing API
  slug: auxen-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-billing-api-openapi.yml
- filename: auxen-ai-deployments-api-openapi.yml
  format: yaml
  label: Auxen Deployments API
  slug: auxen-ai-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-deployments-api-openapi.yml
- filename: auxen-ai-deprecated-api-openapi.yml
  format: yaml
  label: Auxen Deprecated API
  slug: auxen-ai-deprecated-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-deprecated-api-openapi.yml
- filename: auxen-ai-inference-api-openapi.yml
  format: yaml
  label: Auxen Inference API
  slug: auxen-ai-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-inference-api-openapi.yml
- filename: auxen-ai-models-api-openapi.yml
  format: yaml
  label: Auxen Models API
  slug: auxen-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-models-api-openapi.yml
- filename: auxen-ai-pay-with-usdc-api-openapi.yml
  format: yaml
  label: Auxen Pay with USDC API
  slug: auxen-ai-pay-with-usdc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-pay-with-usdc-api-openapi.yml
- filename: auxen-ai-scheduling-api-openapi.yml
  format: yaml
  label: Auxen Scheduling API
  slug: auxen-ai-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-scheduling-api-openapi.yml
- filename: auxen-ai-webhooks-api-openapi.yml
  format: yaml
  label: Auxen Webhooks API
  slug: auxen-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-webhooks-api-openapi.yml
- filename: auxen-ai-workers-api-openapi.yml
  format: yaml
  label: Auxen Workers API
  slug: auxen-ai-workers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auxen-ai/openapi/auxen-ai-workers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Auxen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auxen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Auxen
provider_slug: auxen-ai
scheme_count: 1
schemes:
- description: Bearer token for account-level management key or per-deployment inference key.
  in: header
  name: Authorization
  type: apiKey
slug: auxen-ai-authentication
source_filename: auxen-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://api.auxen.ai/docs/\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token for account-level management key or per-deployment inference key.\n"
source_yaml_url: https://artifacts.apis.io/auxen-ai/authentication/auxen-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Automation
- Platform
- Workers
- Productivity
---
