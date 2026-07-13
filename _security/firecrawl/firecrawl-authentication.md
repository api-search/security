---
api_key_in: []
api_specs:
- filename: firecrawl-openapi-original.json
  format: json
  label: Firecrawl API
  slug: firecrawl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firecrawl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firecrawl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firecrawl
provider_slug: firecrawl
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/firecrawl-openapi-original.json
  type: http
slug: firecrawl-authentication
source_filename: firecrawl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firecrawl-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/firecrawl-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/authentication/firecrawl-authentication.yml
summary_line: http · 1 scheme
tags:
- Crawling
- Data Extraction
- Scraping
- URLs
- AI
- Markdown
---
