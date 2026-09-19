---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: discountedtokens-api-openapi.json
  format: json
  label: DiscountedTokens API
  slug: discountedtokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discountedtokens-api/refs/heads/main/openapi/discountedtokens-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Discountedtokens Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: DiscountedTokens API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DiscountedTokens API
provider_slug: discountedtokens-api
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/discountedtokens-api-openapi.json
  type: http
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/discountedtokens-api-openapi.json
  type: apiKey
slug: discountedtokens-api-authentication
source_filename: discountedtokens-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/discountedtokens-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/discountedtokens-api-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/discountedtokens-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discountedtokens-api/refs/heads/main/authentication/discountedtokens-api-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- LLM
- Generative AI Inference
- OpenAI-Compatible
- Anthropic Compatible
- API Reseller
- Aggregator
- Prepaid
- Usage-Based
- Developer Tools
- AI Infrastructure
---
