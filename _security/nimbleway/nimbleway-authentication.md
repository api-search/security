---
api_key_in: []
api_specs:
- filename: nimbleway-agents-api-openapi.yml
  format: yaml
  label: Nimbleway Agents API
  slug: nimbleway-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-agents-api-openapi.yml
- filename: nimbleway-crawl-api-openapi.yml
  format: yaml
  label: Nimbleway Crawl API
  slug: nimbleway-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-crawl-api-openapi.yml
- filename: nimbleway-domain-knowledge-api-openapi.yml
  format: yaml
  label: Nimbleway Domain Knowledge API
  slug: nimbleway-domain-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-domain-knowledge-api-openapi.yml
- filename: nimbleway-extract-api-openapi.yml
  format: yaml
  label: Nimbleway Extract API
  slug: nimbleway-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-extract-api-openapi.yml
- filename: nimbleway-fast-serp-api-openapi.yml
  format: yaml
  label: Nimbleway Fast SERP API
  slug: nimbleway-fast-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-fast-serp-api-openapi.yml
- filename: nimbleway-jobs-api-openapi.yml
  format: yaml
  label: Nimbleway Jobs API
  slug: nimbleway-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-jobs-api-openapi.yml
- filename: nimbleway-map-api-openapi.yml
  format: yaml
  label: Nimbleway Map API
  slug: nimbleway-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-map-api-openapi.yml
- filename: nimbleway-media-api-openapi.yml
  format: yaml
  label: Nimbleway Media API
  slug: nimbleway-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-media-api-openapi.yml
- filename: nimbleway-search-api-openapi.yml
  format: yaml
  label: Nimbleway Search API
  slug: nimbleway-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-search-api-openapi.yml
- filename: nimbleway-serp-api-openapi.yml
  format: yaml
  label: Nimbleway SERP API
  slug: nimbleway-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-serp-api-openapi.yml
- filename: nimbleway-tasks-api-openapi.yml
  format: yaml
  label: Nimbleway Tasks API
  slug: nimbleway-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nimbleway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nimbleway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nimbleway
provider_slug: nimbleway
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nimbleway-openapi.json
  type: http
slug: nimbleway-authentication
source_filename: nimbleway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nimbleway-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nimbleway-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/authentication/nimbleway-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web Data
- Web Scraping
- Data Extraction
- Web Search
- Proxies
- AI Agents
- MCP
---
