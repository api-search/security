---
anonymous_access: false
api_key_in: []
api_specs:
- filename: libertai-aleph-credits-api-openapi.yml
  format: yaml
  label: LibertAI Aleph Credits API
  slug: libertai-aleph-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-aleph-credits-api-openapi.yml
- filename: libertai-auth-api-openapi.yml
  format: yaml
  label: LibertAI Auth API
  slug: libertai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-auth-api-openapi.yml
- filename: libertai-health-api-openapi.yml
  format: yaml
  label: LibertAI Health API
  slug: libertai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-health-api-openapi.yml
- filename: libertai-models-api-openapi.yml
  format: yaml
  label: LibertAI Models API
  slug: libertai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-models-api-openapi.yml
- filename: libertai-proxy-api-openapi.yml
  format: yaml
  label: LibertAI Proxy API
  slug: libertai-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-proxy-api-openapi.yml
- filename: libertai-search-api-openapi.yml
  format: yaml
  label: LibertAI Search API
  slug: libertai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Libertai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LibertAI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LibertAI
provider_slug: libertai
scheme_count: 2
schemes:
- description: 'Authorization: Bearer $LIBERTAI_API_KEY; keys are created and topped up at https://console.libertai.io'
  name: bearerApiKey
  scheme: bearer
  type: http
- description: Keyless pay-per-request; the API answers 402 Payment Required, the client retries with an EIP-712-signed USDC (Base) payment in the X-PAYMENT header.
  docs: https://docs.libertai.io/apis/x402.html
  name: x402
  type: payment
slug: libertai-authentication
source_filename: libertai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://docs.libertai.io/quickstart.html\ndocs: https://docs.libertai.io/quickstart.html\nnote: The served OpenAPI declares no securitySchemes; the docs document Bearer API keys created in the Developer console, and x402 per-request payment as a keyless alternative.\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer $LIBERTAI_API_KEY; keys are created and topped up at https://console.libertai.io'\n- name: x402\n  type: payment\n  description: Keyless pay-per-request; the API answers 402 Payment Required, the client retries with an EIP-712-signed USDC (Base) payment in the X-PAYMENT header.\n  docs: https://docs.libertai.io/apis/x402.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/authentication/libertai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Inference
- Model Routing
- OpenAI-Compatible
- Decentralized
- Confidential Computing
- x402
---
