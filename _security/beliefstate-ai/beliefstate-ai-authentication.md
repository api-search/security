---
anonymous_access: false
api_key_in: []
api_specs:
- filename: beliefstate-ai-access-api-openapi.yml
  format: yaml
  label: BeliefState Access API
  slug: beliefstate-ai-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-access-api-openapi.yml
- filename: beliefstate-ai-beliefs-api-openapi.yml
  format: yaml
  label: BeliefState Beliefs API
  slug: beliefstate-ai-beliefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-beliefs-api-openapi.yml
- filename: beliefstate-ai-brief-api-openapi.yml
  format: yaml
  label: BeliefState Brief API
  slug: beliefstate-ai-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-brief-api-openapi.yml
- filename: beliefstate-ai-research-api-openapi.yml
  format: yaml
  label: BeliefState Research API
  slug: beliefstate-ai-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-research-api-openapi.yml
- filename: beliefstate-ai-research-payments-api-openapi.yml
  format: yaml
  label: BeliefState Research payments API
  slug: beliefstate-ai-research-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-research-payments-api-openapi.yml
- filename: beliefstate-ai-sources-api-openapi.yml
  format: yaml
  label: BeliefState Sources API
  slug: beliefstate-ai-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-sources-api-openapi.yml
- filename: beliefstate-ai-tickers-api-openapi.yml
  format: yaml
  label: BeliefState Tickers API
  slug: beliefstate-ai-tickers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-tickers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Beliefstate Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BeliefState declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: BeliefState
provider_slug: beliefstate-ai
scheme_count: 4
schemes:
- description: Accountless research tool payments via x402 HTTP header.
  in: header
  name: x402 HTTP
  type: apiKey
- description: MCP authentication with per-tool USDC quotes.
  name: native MCP
  type: oauth2
- description: Account-based REST keys for authenticated access.
  in: header
  name: REST API key
  type: apiKey
- description: OAuth flow for MCP access.
  name: MCP OAuth
  type: oauth2
slug: beliefstate-ai-authentication
source_filename: beliefstate-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://docs.beliefstate.ai/guides/authentication.md\nschemes:\n  - name: x402 HTTP\n    type: apiKey\n    in: header\n    description: Accountless research tool payments via x402 HTTP header.\n  - name: native MCP\n    type: oauth2\n    description: MCP authentication with per-tool USDC quotes.\n  - name: REST API key\n    type: apiKey\n    in: header\n    description: Account-based REST keys for authenticated access.\n  - name: MCP OAuth\n    type: oauth2\n    description: OAuth flow for MCP access.\n"
source_yaml_url: https://artifacts.apis.io/beliefstate-ai/authentication/beliefstate-ai-authentication.yml
summary_line: 4 schemes
tags:
- Artificial Intelligence
- Finance
- Research
- Analytics
- Platform
---
