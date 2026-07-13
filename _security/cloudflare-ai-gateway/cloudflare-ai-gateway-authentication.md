---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudflare Ai Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudflare AI Gateway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudflare AI Gateway
provider_slug: cloudflare-ai-gateway
scheme_count: 1
schemes:
- description: 'Cloudflare API token with AI Gateway Read/Edit (and Workers AI Read

    when applicable) permissions, passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudflare-ai-gateway-openapi.yml
  type: http
slug: cloudflare-ai-gateway-authentication
source_filename: cloudflare-ai-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudflare-ai-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Cloudflare API token with AI Gateway Read/Edit (and Workers AI Read\n    when applicable) permissions, passed as `Authorization: Bearer <token>`.\n  sources:\n  - openapi/cloudflare-ai-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-ai-gateway/refs/heads/main/authentication/cloudflare-ai-gateway-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Gateway
- LLM
- Observability
- Caching
- Rate Limiting
- Workers AI
- Cloudflare
---
