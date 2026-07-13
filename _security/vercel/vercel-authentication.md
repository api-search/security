---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Vercel REST API
  slug: vercel-rest-api
  spec_type: OpenAPI
  url: https://openapi.vercel.sh/
- filename: vercel-ai-gateway-openapi.yml
  format: yaml
  label: Vercel AI Gateway API
  slug: vercel-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-ai-gateway-openapi.yml
- filename: vercel-webhooks-asyncapi.yml
  format: yaml
  label: Vercel Webhooks
  slug: vercel-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/asyncapi/vercel-webhooks-asyncapi.yml
- filename: vercel-v0-platform-openapi.yml
  format: yaml
  label: V0 Platform API
  slug: v0-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-v0-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vercel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vercel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vercel
provider_slug: vercel
scheme_count: 1
schemes:
- description: Vercel AI Gateway API key (AI_GATEWAY_API_KEY)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vercel-ai-gateway-openapi.yml
  - openapi/vercel-v0-platform-openapi.yml
  type: http
slug: vercel-authentication
source_filename: vercel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vercel-ai-gateway-openapi.yml, openapi/vercel-v0-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Vercel AI Gateway API key (AI_GATEWAY_API_KEY)\n  sources:\n  - openapi/vercel-ai-gateway-openapi.yml\n  - openapi/vercel-v0-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/authentication/vercel-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Gateways
- Gateways
- Observability
- Webhooks
---
