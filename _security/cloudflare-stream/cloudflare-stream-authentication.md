---
api_key_in: []
api_specs:
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Videos API
  slug: cloudflare-stream-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Live Inputs API
  slug: cloudflare-stream-live-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Captions API
  slug: cloudflare-stream-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Signed URLs API
  slug: cloudflare-stream-signed-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Webhooks API
  slug: cloudflare-stream-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Analytics API
  slug: cloudflare-stream-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudflare Stream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudflare Stream secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudflare Stream
provider_slug: cloudflare-stream
scheme_count: 1
schemes:
- description: Cloudflare API token passed in an Authorization Bearer header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudflare-stream-openapi.yml
  type: http
slug: cloudflare-stream-authentication
source_filename: cloudflare-stream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudflare-stream-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Cloudflare API token passed in an Authorization Bearer header.\n  sources:\n  - openapi/cloudflare-stream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/authentication/cloudflare-stream-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Live Streaming
- Media
- Video Hosting
- Cloudflare
---
