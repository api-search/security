---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xpoz-ai-account-api-openapi.yml
  format: yaml
  label: xpoz-ai Account API
  slug: xpoz-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-account-api-openapi.yml
- filename: xpoz-ai-billing-api-openapi.yml
  format: yaml
  label: xpoz-ai Billing API
  slug: xpoz-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-billing-api-openapi.yml
- filename: xpoz-ai-crawl-settings-api-openapi.yml
  format: yaml
  label: xpoz-ai Crawl Settings API
  slug: xpoz-ai-crawl-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-crawl-settings-api-openapi.yml
- filename: xpoz-ai-instagram-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Instagram (live) API
  slug: xpoz-ai-instagram-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-instagram-live-api-openapi.yml
- filename: xpoz-ai-operations-api-openapi.yml
  format: yaml
  label: xpoz-ai Operations API
  slug: xpoz-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-operations-api-openapi.yml
- filename: xpoz-ai-platform-api-openapi.yml
  format: yaml
  label: xpoz-ai Platform API
  slug: xpoz-ai-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-platform-api-openapi.yml
- filename: xpoz-ai-reddit-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Reddit (live) API
  slug: xpoz-ai-reddit-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-reddit-live-api-openapi.yml
- filename: xpoz-ai-system-status-api-openapi.yml
  format: yaml
  label: xpoz-ai System Status API
  slug: xpoz-ai-system-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-system-status-api-openapi.yml
- filename: xpoz-ai-tiktok-live-api-openapi.yml
  format: yaml
  label: xpoz-ai TikTok (live) API
  slug: xpoz-ai-tiktok-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-tiktok-live-api-openapi.yml
- filename: xpoz-ai-twitter-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Twitter (live) API
  slug: xpoz-ai-twitter-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-twitter-live-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: xpoz-ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: xpoz-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: xpoz-ai
provider_slug: xpoz-ai
scheme_count: 1
schemes:
- description: 'XPOZ API access key, created from the dashboard or `POST /api/tokens`. Send as `Authorization: Bearer <access key>`.'
  name: AccessKey
  scheme: bearer
  sources:
  - openapi/xpoz-ai-openapi.json
  type: http
slug: xpoz-ai-authentication
source_filename: xpoz-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/xpoz-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AccessKey\n  type: http\n  scheme: bearer\n  description: 'XPOZ API access key, created from the dashboard or `POST /api/tokens`. Send\n    as `Authorization: Bearer <access key>`.'\n  sources:\n  - openapi/xpoz-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/xpoz-ai/authentication/xpoz-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Social Data
- Artificial Intelligence
- Monitoring
- Analytics
- SDK
---
