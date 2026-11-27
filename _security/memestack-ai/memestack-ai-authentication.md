---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: memestack-ai-account-api-openapi.yml
  format: yaml
  label: MemeStack Account API
  slug: memestack-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-account-api-openapi.yml
- filename: memestack-ai-agent-payments-api-openapi.yml
  format: yaml
  label: MemeStack Agent payments API
  slug: memestack-ai-agent-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-agent-payments-api-openapi.yml
- filename: memestack-ai-collections-api-openapi.yml
  format: yaml
  label: MemeStack Collections API
  slug: memestack-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-collections-api-openapi.yml
- filename: memestack-ai-developer-account-api-openapi.yml
  format: yaml
  label: MemeStack Developer account API
  slug: memestack-ai-developer-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-developer-account-api-openapi.yml
- filename: memestack-ai-developer-api-api-openapi.yml
  format: yaml
  label: MemeStack Developer API
  slug: memestack-ai-developer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-developer-api-api-openapi.yml
- filename: memestack-ai-feedback-api-openapi.yml
  format: yaml
  label: MemeStack Feedback API
  slug: memestack-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-feedback-api-openapi.yml
- filename: memestack-ai-generation-api-openapi.yml
  format: yaml
  label: MemeStack Generation API
  slug: memestack-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-generation-api-openapi.yml
- filename: memestack-ai-images-api-openapi.yml
  format: yaml
  label: MemeStack Images API
  slug: memestack-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-images-api-openapi.yml
- filename: memestack-ai-imports-api-openapi.yml
  format: yaml
  label: MemeStack Imports API
  slug: memestack-ai-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-imports-api-openapi.yml
- filename: memestack-ai-leaderboard-api-openapi.yml
  format: yaml
  label: MemeStack Leaderboard API
  slug: memestack-ai-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-leaderboard-api-openapi.yml
- filename: memestack-ai-memeverse-api-openapi.yml
  format: yaml
  label: MemeStack Memeverse API
  slug: memestack-ai-memeverse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-memeverse-api-openapi.yml
- filename: memestack-ai-premium-and-prices-api-openapi.yml
  format: yaml
  label: MemeStack Premium and prices API
  slug: memestack-ai-premium-and-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-premium-and-prices-api-openapi.yml
- filename: memestack-ai-reports-and-takedowns-api-openapi.yml
  format: yaml
  label: MemeStack Reports and takedowns API
  slug: memestack-ai-reports-and-takedowns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-reports-and-takedowns-api-openapi.yml
- filename: memestack-ai-search-api-openapi.yml
  format: yaml
  label: MemeStack Search API
  slug: memestack-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-search-api-openapi.yml
- filename: memestack-ai-service-api-openapi.yml
  format: yaml
  label: MemeStack Service API
  slug: memestack-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-service-api-openapi.yml
- filename: memestack-ai-tags-api-openapi.yml
  format: yaml
  label: MemeStack Tags API
  slug: memestack-ai-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-tags-api-openapi.yml
- filename: memestack-ai-uploads-api-openapi.yml
  format: yaml
  label: MemeStack Uploads API
  slug: memestack-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-uploads-api-openapi.yml
- filename: memestack-ai-users-api-openapi.yml
  format: yaml
  label: MemeStack Users API
  slug: memestack-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-users-api-openapi.yml
- filename: memestack-ai-zaps-api-openapi.yml
  format: yaml
  label: MemeStack Zaps API
  slug: memestack-ai-zaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memestack-ai/openapi/memestack-ai-zaps-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: MemeStack Authentication
name_suffix: Authentication
oauth_flows: []
overview: MemeStack secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MemeStack
provider_slug: memestack-ai
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: JWT issued by /auth/callback (LNURL) or /auth/email/verify. Also accepted as the httpOnly cookie __Secure-bii-token for same-origin browser requests.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/memestack-ai-openapi.json
  type: http
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/memestack-ai-openapi.json
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/memestack-ai-openapi.json
  type: apiKey
slug: memestack-ai-authentication
source_filename: memestack-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/memestack-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT issued by /auth/callback (LNURL) or /auth/email/verify. Also accepted as\n    the httpOnly cookie __Secure-bii-token for same-origin browser requests.\n  sources:\n  - openapi/memestack-ai-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/memestack-ai-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/memestack-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/memestack-ai/authentication/memestack-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Visual Search
- Memes
- Infographics
- Charts
- Community
---
