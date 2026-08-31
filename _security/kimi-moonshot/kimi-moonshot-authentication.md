---
api_key_in: []
api_specs:
- filename: kimi-moonshot-batch-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Batch API
  slug: kimi-moonshot-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-batch-api-openapi.yml
- filename: kimi-moonshot-billing-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Billing API
  slug: kimi-moonshot-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-billing-api-openapi.yml
- filename: kimi-moonshot-chat-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Chat API
  slug: kimi-moonshot-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-chat-api-openapi.yml
- filename: kimi-moonshot-files-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Files API
  slug: kimi-moonshot-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-files-api-openapi.yml
- filename: kimi-moonshot-models-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Models API
  slug: kimi-moonshot-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-models-api-openapi.yml
- filename: kimi-moonshot-utilities-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Utilities API
  slug: kimi-moonshot-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-utilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kimi Moonshot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kimi (Moonshot AI) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kimi (Moonshot AI)
provider_slug: kimi-moonshot
scheme_count: 1
schemes:
- description: Authorization 请求头需要一个 Bearer 令牌。使用 MOONSHOT_API_KEY 作为令牌。这是一个服务端密钥，请在 [API 密钥页面](https://platform.kimi.com/console/api-keys) 生成。
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kimi-moonshot-openapi.json
  type: http
slug: kimi-moonshot-authentication
source_filename: kimi-moonshot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kimi-moonshot-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authorization 请求头需要一个 Bearer 令牌。使用 MOONSHOT_API_KEY 作为令牌。这是一个服务端密钥，请在 [API 密钥页面](https://platform.kimi.com/console/api-keys)\n    生成。\n  sources:\n  - openapi/kimi-moonshot-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/authentication/kimi-moonshot-authentication.yml
summary_line: http · 1 scheme
tags:
- LLM
- Long Context
- Artificial Intelligence
- OpenAI-Compatible
- Multimodal
- China
---
