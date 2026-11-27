---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ioswarm-io-auth-api-openapi.yml
  format: yaml
  label: Swarmio Auth API
  slug: ioswarm-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-auth-api-openapi.yml
- filename: ioswarm-io-billing-api-openapi.yml
  format: yaml
  label: Swarmio Billing API
  slug: ioswarm-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-billing-api-openapi.yml
- filename: ioswarm-io-feeds-api-openapi.yml
  format: yaml
  label: Swarmio Feeds API
  slug: ioswarm-io-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-feeds-api-openapi.yml
- filename: ioswarm-io-llms-txt-api-openapi.yml
  format: yaml
  label: Swarmio Llms.txt API
  slug: ioswarm-io-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-llms-txt-api-openapi.yml
- filename: ioswarm-io-market-api-openapi.yml
  format: yaml
  label: Swarmio Market API
  slug: ioswarm-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-market-api-openapi.yml
- filename: ioswarm-io-news-api-openapi.yml
  format: yaml
  label: Swarmio News API
  slug: ioswarm-io-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-news-api-openapi.yml
- filename: ioswarm-io-pulse-api-openapi.yml
  format: yaml
  label: Swarmio Pulse API
  slug: ioswarm-io-pulse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-pulse-api-openapi.yml
- filename: ioswarm-io-search-api-openapi.yml
  format: yaml
  label: Swarmio Search API
  slug: ioswarm-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-search-api-openapi.yml
- filename: ioswarm-io-video-api-openapi.yml
  format: yaml
  label: Swarmio Video API
  slug: ioswarm-io-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-video-api-openapi.yml
- filename: ioswarm-io-x402-api-openapi.yml
  format: yaml
  label: Swarmio X402 API
  slug: ioswarm-io-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioswarm-io/openapi/ioswarm-io-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Swarmio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swarmio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swarmio
provider_slug: ioswarm-io
scheme_count: 1
schemes:
- description: An sk_swarm_ API key (long-lived; self-mint via /api/v1/account/api-keys) or a Supabase access_token (short-lived; from signup).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ioswarm-io-openapi.json
  type: http
slug: ioswarm-io-authentication
source_filename: ioswarm-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/ioswarm-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An sk_swarm_ API key (long-lived; self-mint via /api/v1/account/api-keys) or\n    a Supabase access_token (short-lived; from signup).\n  sources:\n  - openapi/ioswarm-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ioswarm-io/authentication/ioswarm-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Deep Research
- News Briefs
- Finance
- Product Comparisons
- Trip Planning
- Design Studio
- Hosted Harness
---
