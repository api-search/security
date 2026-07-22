---
api_key_in:
- header
api_specs:
- filename: mindlogic-api-gateway-openapi-original.json
  format: json
  label: FactChat API Gateway
  slug: factchat-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-api-gateway-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mindlogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mindlogic secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mindlogic
provider_slug: mindlogic
scheme_count: 2
schemes:
- default_for: OpenAI SDK and OpenAI-compatible clients
  format: 'Authorization: Bearer <API_KEY>'
  in: header
  name: BearerApiKey
  scheme_header: Authorization
  sources:
  - docs
  type: apiKey
- default_for: Anthropic SDK and Claude clients
  format: 'x-api-key: <API_KEY>'
  in: header
  name: XApiKey
  parameter_name: x-api-key
  sources:
  - docs
  type: apiKey
slug: mindlogic-authentication
source_filename: mindlogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mindlogic.ai/docs/general/api-gateway/getting-started/authentication\ndocs: https://docs.mindlogic.ai/docs/general/api-gateway/getting-started/authentication\nnote: >-\n  The harvested OpenAPI (openapi/mindlogic-api-gateway-openapi-original.json)\n  declares no securitySchemes, but the Gateway is API-key authenticated per the\n  docs and confirmed by a live 401 (\"Bearer token is not supplied\"). This\n  profile is sourced from the documentation.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: BearerApiKey\n    type: apiKey\n    in: header\n    scheme_header: Authorization\n    format: \"Authorization: Bearer <API_KEY>\"\n    default_for: OpenAI SDK and OpenAI-compatible clients\n    sources: [docs]\n  - name: XApiKey\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    format: \"x-api-key: <API_KEY>\"\n    default_for: Anthropic SDK and Claude clients\n\
  \    sources: [docs]\nkey_management:\n  how_to_obtain: >-\n    Log into the FactChat website, open API Gateway in the left sidebar, click\n    the API-key generation button, then copy and securely store the key.\n  console: https://docs.mindlogic.ai/docs/general/api-gateway/getting-started/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/authentication/mindlogic-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI/ML
- Generative AI
- Conversational AI
- LLM Gateway
- Chatbots
- API Gateway
- Korea
---
