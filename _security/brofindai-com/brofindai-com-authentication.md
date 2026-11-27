---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brofindai-com-agents-api-openapi.yml
  format: yaml
  label: Bro Find AI Agents API
  slug: brofindai-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-agents-api-openapi.yml
- filename: brofindai-com-badge-api-openapi.yml
  format: yaml
  label: Bro Find AI Badge API
  slug: brofindai-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-badge-api-openapi.yml
- filename: brofindai-com-comments-api-openapi.yml
  format: yaml
  label: Bro Find AI Comments API
  slug: brofindai-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-comments-api-openapi.yml
- filename: brofindai-com-feedback-api-openapi.yml
  format: yaml
  label: Bro Find AI Feedback API
  slug: brofindai-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-feedback-api-openapi.yml
- filename: brofindai-com-mcp-servers-api-openapi.yml
  format: yaml
  label: Bro Find AI MCP Servers API
  slug: brofindai-com-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-mcp-servers-api-openapi.yml
- filename: brofindai-com-reviews-api-openapi.yml
  format: yaml
  label: Bro Find AI Reviews API
  slug: brofindai-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-reviews-api-openapi.yml
- filename: brofindai-com-search-api-openapi.yml
  format: yaml
  label: Bro Find AI Search API
  slug: brofindai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-search-api-openapi.yml
- filename: brofindai-com-tools-api-openapi.yml
  format: yaml
  label: Bro Find AI Tools API
  slug: brofindai-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-tools-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bro Find AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bro Find AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bro Find AI
provider_slug: brofindai-com
scheme_count: 1
schemes:
- bearerFormat: Firebase ID Token
  description: Firebase Authentication ID token obtained via Google Sign-In
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/brofindai-com-openapi.json
  type: http
slug: brofindai-com-authentication
source_filename: brofindai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/brofindai-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Firebase ID Token\n  description: Firebase Authentication ID token obtained via Google Sign-In\n  sources:\n  - openapi/brofindai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/brofindai-com/authentication/brofindai-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Directory
- Tools
- Marketplace
- Company
---
