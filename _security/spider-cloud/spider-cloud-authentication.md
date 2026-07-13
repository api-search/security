---
api_key_in: []
api_specs:
- filename: spider-cloud-openapi.yml
  format: yaml
  label: Spider API
  slug: spider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spider Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spider secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spider
provider_slug: spider-cloud
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spider-cloud-openapi.yml
  type: http
slug: spider-cloud-authentication
source_filename: spider-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spider-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/spider-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/authentication/spider-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Crawling
- Scraping
- Data Extraction
- URLs
- AI
- Markdown
- MCP
- Rust
- Headless Browser
- Proxies
---
