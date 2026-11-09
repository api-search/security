---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentgates-ai-compute-api-openapi.yml
  format: yaml
  label: Agentgates Compute API
  slug: agentgates-ai-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-compute-api-openapi.yml
- filename: agentgates-ai-directory-api-openapi.yml
  format: yaml
  label: Agentgates Directory API
  slug: agentgates-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-directory-api-openapi.yml
- filename: agentgates-ai-inference-api-openapi.yml
  format: yaml
  label: Agentgates Inference API
  slug: agentgates-ai-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-inference-api-openapi.yml
- filename: agentgates-ai-llms-txt-api-openapi.yml
  format: yaml
  label: Agentgates Llms.txt API
  slug: agentgates-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-llms-txt-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agentgates Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentgates declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agentgates
provider_slug: agentgates-ai
scheme_count: 3
schemes:
- description: Anonymous payment signature identifies the wallet; used as authentication.
  name: x402-payment-signature
  type: custom
- description: Bearer key minted on a prepaid balance, revocable.
  name: revocable-bearer-key
  type: bearer
- description: Standard OAuth flow for wallet MCP server.
  name: OAuth
  type: oauth2
slug: agentgates-ai-authentication
source_filename: agentgates-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agentgates.ai/docs/api-without-api-keys-wallet-auth\nschemes:\n  - type: custom\n    name: x402-payment-signature\n    description: Anonymous payment signature identifies the wallet; used as authentication.\n  - type: bearer\n    name: revocable-bearer-key\n    description: Bearer key minted on a prepaid balance, revocable.\n  - type: oauth2\n    name: OAuth\n    description: Standard OAuth flow for wallet MCP server.\n"
source_yaml_url: https://artifacts.apis.io/agentgates-ai/authentication/agentgates-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Compute
- Inference
- Blockchain
- Payments
---
