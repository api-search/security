---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mistralai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mistral AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mistral AI
provider_slug: mistralai
scheme_count: 1
schemes:
- description: All Mistral AI La Plateforme endpoints authenticate with a personal API key issued from the console (https://console.mistral.ai) and sent as an HTTP Bearer token in the Authorization header. There is no OAuth or OIDC surface on the inference API.
  format: 'Authorization: Bearer $MISTRAL_API_KEY'
  header: Authorization
  in: header
  name: ApiKey
  scheme: bearer
  sources:
  - https://docs.mistral.ai/getting-started/quickstart
  type: http
slug: mistralai-authentication
source_filename: mistralai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mistral.ai/getting-started/quickstart\ndocs: https://docs.mistral.ai/api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\nschemes:\n  - name: ApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Authorization: Bearer $MISTRAL_API_KEY\"\n    description: >-\n      All Mistral AI La Plateforme endpoints authenticate with a personal API key\n      issued from the console (https://console.mistral.ai) and sent as an\n      HTTP Bearer token in the Authorization header. There is no OAuth or OIDC\n      surface on the inference API.\n    sources: [https://docs.mistral.ai/getting-started/quickstart]\nnotes: >-\n  Derived from Mistral AI public authentication documentation; this repo holds no\n  local OpenAPI, so the profile is captured from docs rather than a spec derive.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistralai/refs/heads/main/authentication/mistralai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Generative AI
- Machine Learning
- Chat
- Embeddings
- Agents
- OCR
- Fine-Tuning
- Developer Platform
---
