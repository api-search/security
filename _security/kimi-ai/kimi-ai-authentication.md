---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kimi-ai-batch-api-openapi.yml
  format: yaml
  label: Moonshot AI Batch API
  slug: kimi-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-batch-api-openapi.yml
- filename: kimi-ai-billing-api-openapi.yml
  format: yaml
  label: Moonshot AI Billing API
  slug: kimi-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-billing-api-openapi.yml
- filename: kimi-ai-files-api-openapi.yml
  format: yaml
  label: Moonshot AI Files API
  slug: kimi-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-files-api-openapi.yml
- filename: kimi-ai-models-api-openapi.yml
  format: yaml
  label: Moonshot AI Models API
  slug: kimi-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-models-api-openapi.yml
- filename: kimi-ai-utilities-api-openapi.yml
  format: yaml
  label: Moonshot AI Utilities API
  slug: kimi-ai-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-utilities-api-openapi.yml
- filename: kimi-ai-responses-api-openapi.yml
  format: yaml
  label: Moonshot AI Responses API
  slug: kimi-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-responses-api-openapi.yml
- filename: kimi-ai-tools-api-openapi.yml
  format: yaml
  label: Moonshot AI Tools API
  slug: kimi-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-tools-api-openapi.yml
- filename: kimi-ai-messages-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Messages API
  slug: kimi-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-messages-api-openapi.yml
- filename: kimi-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Chat Completions API
  slug: kimi-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kimi Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kimi (Moonshot AI) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kimi (Moonshot AI)
provider_slug: kimi-ai
scheme_count: 1
schemes:
- description: All API requests require an API Key in the HTTP header. API Keys are created and managed in the Kimi Open Platform Console (https://platform.kimi.ai/console/api-keys). Server-side secret; do not expose in client-side code.
  header: 'Authorization: Bearer $MOONSHOT_API_KEY'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/
  - https://platform.kimi.ai/docs/api/overview.md
  type: http
slug: kimi-ai-authentication
source_filename: kimi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: searched\nsource: https://platform.kimi.ai/docs/api/overview.md\ndocs:\n- https://platform.kimi.ai/docs/api/overview.md\n- https://platform.kimi.ai/docs/get-your-api-key.md\n- https://platform.kimi.ai/docs/guide/org-best-practice.md\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer $MOONSHOT_API_KEY'\n  description: All API requests require an API Key in the HTTP header. API Keys are created and managed in the Kimi Open Platform Console (https://platform.kimi.ai/console/api-keys). Server-side secret;\n    do not expose in client-side code.\n  sources:\n  - openapi/\n  - https://platform.kimi.ai/docs/api/overview.md\nnotes:\n- Same key works against the Anthropic-compatible base_url https://api.moonshot.ai/anthropic.\n- Keys issued on platform.kimi.ai are independent from keys on other regional Kimi platforms; mixing returns 401 (errors page).\n- Organization-level IP\
  \ whitelist can restrict API access per organization; disallowed IPs get 403 \"Your IP is not allowed to access this organization\".\n- No OAuth 2.0 or scopes are documented.\n"
source_yaml_url: https://artifacts.apis.io/kimi-ai/authentication/kimi-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Inference
- Long Context
- Kimi
- Foundation Models
---
