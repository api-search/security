---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: howgooditcanget-com-clarity-os-api-openapi.yml
  format: yaml
  label: How Good It Can Get Clarity OS API
  slug: howgooditcanget-com-clarity-os-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howgooditcanget-com/openapi/howgooditcanget-com-clarity-os-api-openapi.yml
- filename: howgooditcanget-com-clarity-os-mcp-api-openapi.yml
  format: yaml
  label: How Good It Can Get Clarity OS MCP API
  slug: howgooditcanget-com-clarity-os-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howgooditcanget-com/openapi/howgooditcanget-com-clarity-os-mcp-api-openapi.yml
- filename: howgooditcanget-com-health-api-openapi.yml
  format: yaml
  label: How Good It Can Get Health API
  slug: howgooditcanget-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howgooditcanget-com/openapi/howgooditcanget-com-health-api-openapi.yml
- filename: howgooditcanget-com-knowledge-api-openapi.yml
  format: yaml
  label: How Good It Can Get Knowledge API
  slug: howgooditcanget-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howgooditcanget-com/openapi/howgooditcanget-com-knowledge-api-openapi.yml
- filename: howgooditcanget-com-mcp-api-openapi.yml
  format: yaml
  label: How Good It Can Get MCP API
  slug: howgooditcanget-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howgooditcanget-com/openapi/howgooditcanget-com-mcp-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: How Good It Can Get Authentication
name_suffix: Authentication
oauth_flows: []
overview: How Good It Can Get secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: How Good It Can Get
provider_slug: howgooditcanget-com
scheme_count: 2
schemes:
- description: Canonical x402 V2 payment signature for separately governed paid resources.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/howgooditcanget-com-openapi.json
  type: apiKey
- description: Legacy x402 compatibility header. New integrations should use PAYMENT-SIGNATURE.
  in: header
  name: x402LegacyPayment
  parameter: X-Payment
  sources:
  - openapi/howgooditcanget-com-openapi.json
  type: apiKey
slug: howgooditcanget-com-authentication
source_filename: howgooditcanget-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/howgooditcanget-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Canonical x402 V2 payment signature for separately governed paid resources.\n  sources:\n  - openapi/howgooditcanget-com-openapi.json\n- name: x402LegacyPayment\n  type: apiKey\n  in: header\n  parameter: X-Payment\n  description: Legacy x402 compatibility header. New integrations should use PAYMENT-SIGNATURE.\n  sources:\n  - openapi/howgooditcanget-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/howgooditcanget-com/authentication/howgooditcanget-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Real-Time
- Pattern-Interruption
- Clarity-Protocol
- Business Intelligence
---
