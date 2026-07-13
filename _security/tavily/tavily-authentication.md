---
api_key_in: []
api_specs:
- filename: tavily-openapi.yml
  format: yaml
  label: Tavily Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavily/refs/heads/main/openapi/tavily-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tavily Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tavily secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tavily
provider_slug: tavily
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tavily-openapi.yml
  type: http
slug: tavily-authentication
source_filename: tavily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tavily-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/tavily-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tavily/refs/heads/main/authentication/tavily-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Web Search
- AI Agents
- LLMs
- Extract
- Crawl
- Sitemap
- Research
- REST
- LangChain
- LlamaIndex
- Real-Time
---
