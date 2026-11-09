---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agentcreditdata-com-agent-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Agent API
  slug: agentcreditdata-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-agent-api-openapi.yml
- filename: agentcreditdata-com-assess-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Assess API
  slug: agentcreditdata-com-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-assess-api-openapi.yml
- filename: agentcreditdata-com-verify-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Verify API
  slug: agentcreditdata-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentcreditdata Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Credit Bureau secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agent Credit Bureau
provider_slug: agentcreditdata-com
scheme_count: 1
schemes:
- description: Base64 x402 v2 PaymentPayload; receipt returned in PAYMENT-RESPONSE.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/agentcreditdata-com-openapi.json
  type: apiKey
slug: agentcreditdata-com-authentication
source_filename: agentcreditdata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentcreditdata-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Base64 x402 v2 PaymentPayload; receipt returned in PAYMENT-RESPONSE.\n  sources:\n  - openapi/agentcreditdata-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentcreditdata-com/authentication/agentcreditdata-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Finance
- Credit
- Artificial Intelligence
- Data
---
