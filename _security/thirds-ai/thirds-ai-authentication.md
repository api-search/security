---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: thirds-ai-batches-api-openapi.yml
  format: yaml
  label: thirds.ai Batches API
  slug: thirds-ai-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-batches-api-openapi.yml
- filename: thirds-ai-brand-kits-api-openapi.yml
  format: yaml
  label: thirds.ai Brand Kits API
  slug: thirds-ai-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-brand-kits-api-openapi.yml
- filename: thirds-ai-carousels-api-openapi.yml
  format: yaml
  label: thirds.ai Carousels API
  slug: thirds-ai-carousels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-carousels-api-openapi.yml
- filename: thirds-ai-downloads-api-openapi.yml
  format: yaml
  label: thirds.ai Downloads API
  slug: thirds-ai-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-downloads-api-openapi.yml
- filename: thirds-ai-image-api-openapi.yml
  format: yaml
  label: thirds.ai Image API
  slug: thirds-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-image-api-openapi.yml
- filename: thirds-ai-image-assets-api-openapi.yml
  format: yaml
  label: thirds.ai Image Assets API
  slug: thirds-ai-image-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-image-assets-api-openapi.yml
- filename: thirds-ai-image-packs-api-openapi.yml
  format: yaml
  label: thirds.ai Image Packs API
  slug: thirds-ai-image-packs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-image-packs-api-openapi.yml
- filename: thirds-ai-keys-api-openapi.yml
  format: yaml
  label: thirds.ai Keys API
  slug: thirds-ai-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-keys-api-openapi.yml
- filename: thirds-ai-me-api-openapi.yml
  format: yaml
  label: thirds.ai Me API
  slug: thirds-ai-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-me-api-openapi.yml
- filename: thirds-ai-openapi-json-api-openapi.yml
  format: yaml
  label: thirds.ai Openapi.json API
  slug: thirds-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-openapi-json-api-openapi.yml
- filename: thirds-ai-pdf-api-openapi.yml
  format: yaml
  label: thirds.ai PDF API
  slug: thirds-ai-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-pdf-api-openapi.yml
- filename: thirds-ai-public-stats-api-openapi.yml
  format: yaml
  label: thirds.ai Public Stats API
  slug: thirds-ai-public-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-public-stats-api-openapi.yml
- filename: thirds-ai-template-builds-api-openapi.yml
  format: yaml
  label: thirds.ai Template Builds API
  slug: thirds-ai-template-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-template-builds-api-openapi.yml
- filename: thirds-ai-templates-api-openapi.yml
  format: yaml
  label: thirds.ai Templates API
  slug: thirds-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-templates-api-openapi.yml
- filename: thirds-ai-testimonials-api-openapi.yml
  format: yaml
  label: thirds.ai Testimonials API
  slug: thirds-ai-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-testimonials-api-openapi.yml
- filename: thirds-ai-webhooks-api-openapi.yml
  format: yaml
  label: thirds.ai Webhooks API
  slug: thirds-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Thirds Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: thirds.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: thirds.ai
provider_slug: thirds-ai
scheme_count: 2
schemes:
- description: A browser session. Browser writes also require the matching x-csrf-token header from GET /v1/me.
  in: cookie
  name: sessionCookie
  parameter: __Host-thirds_session
  sources:
  - openapi/thirds-ai-openapi.yml
  type: apiKey
- description: 'An API key''s secret, sent as "Authorization: Bearer thirds_sk_v1_...".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thirds-ai-openapi.yml
  type: http
slug: thirds-ai-authentication
source_filename: thirds-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/thirds-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __Host-thirds_session\n  description: A browser session. Browser writes also require the matching x-csrf-token header\n    from GET /v1/me.\n  sources:\n  - openapi/thirds-ai-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key''s secret, sent as \"Authorization: Bearer thirds_sk_v1_...\".'\n  sources:\n  - openapi/thirds-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/authentication/thirds-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- pdf-automation
- image-automation
- Document Generation
- HTML to PDF
- HTML to Image
- template-rendering
- Branded Content
- Developer Tools
- MCP Server
- Agent-Native
- marketing-ops
---
