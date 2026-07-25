---
api_key_in: []
api_specs:
- filename: scrunch-ai-agent-traffic-api-openapi.yml
  format: yaml
  label: Scrunch AI agent-traffic API
  slug: scrunch-ai-agent-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-agent-traffic-api-openapi.yml
- filename: scrunch-ai-ai-referrals-api-openapi.yml
  format: yaml
  label: Scrunch AI ai-referrals API
  slug: scrunch-ai-ai-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-ai-referrals-api-openapi.yml
- filename: scrunch-ai-axp-render-api-openapi.yml
  format: yaml
  label: Scrunch AI axp-render API
  slug: scrunch-ai-axp-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-axp-render-api-openapi.yml
- filename: scrunch-ai-brands-api-openapi.yml
  format: yaml
  label: Scrunch AI Brands API
  slug: scrunch-ai-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-brands-api-openapi.yml
- filename: scrunch-ai-orchestration-api-openapi.yml
  format: yaml
  label: Scrunch AI orchestration API
  slug: scrunch-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-orchestration-api-openapi.yml
- filename: scrunch-ai-page-audits-api-openapi.yml
  format: yaml
  label: Scrunch AI Page Audits API
  slug: scrunch-ai-page-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-page-audits-api-openapi.yml
- filename: scrunch-ai-prompts-api-openapi.yml
  format: yaml
  label: Scrunch AI Prompts API
  slug: scrunch-ai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-prompts-api-openapi.yml
- filename: scrunch-ai-query-api-openapi.yml
  format: yaml
  label: Scrunch AI Query API
  slug: scrunch-ai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-query-api-openapi.yml
- filename: scrunch-ai-responses-api-openapi.yml
  format: yaml
  label: Scrunch AI Responses API
  slug: scrunch-ai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-responses-api-openapi.yml
- filename: scrunch-ai-sitemap-api-openapi.yml
  format: yaml
  label: Scrunch AI sitemap API
  slug: scrunch-ai-sitemap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-sitemap-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Scrunch Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scrunch AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scrunch AI
provider_slug: scrunch-ai
scheme_count: 1
schemes:
- format: Bearer <SCRUNCH_API_TOKEN>
  header: Authorization
  in: header
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/scrunch-ai-data-api-openapi.yml
  type: http
slug: scrunch-ai-authentication
source_filename: scrunch-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scrunch-ai-data-api-openapi.yml\ndocs: https://developers.scrunch.com/getting-started/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_model: api-key\n  scopes:\n  - query\n  - configure\n  - create-brand\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <SCRUNCH_API_TOKEN>'\n  sources:\n  - openapi/scrunch-ai-data-api-openapi.yml\nnotes: |\n  All Scrunch Data API endpoints require a Bearer token in the Authorization header.\n  API keys are provisioned at the organization level under Organization -> Settings ->\n  API Keys and are shown only once at creation time. Keys carry operational scopes\n  (Query / Configure / Create Brand) and a brand access grant: brand-scoped keys can\n  only access specific brands, organization-scoped keys can access and configure all\n  brands. API key creation is gated to the Agency and\
  \ Enterprise plans; calling\n  POST /organizations/{organization_id}/api-keys without the required plan capability\n  returns HTTP 402 Payment Required.\n  Note: the hosted Scrunch MCP server (Scrunchie) uses OAuth sign-in instead of API keys\n  (see mcp/scrunch-ai-mcp.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/authentication/scrunch-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- AI Search
- Answer Engine Optimization
- Generative Engine Optimization
- Brand Visibility
- Analytics
- SEO
- Agent Experience
- MCP
---
