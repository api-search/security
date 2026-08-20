---
api_key_in: []
api_specs:
- filename: spider-cloud-crawling-api-openapi.yml
  format: yaml
  label: Spider Crawling API
  slug: spider-cloud-crawling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-crawling-api-openapi.yml
- filename: spider-cloud-data-api-openapi.yml
  format: yaml
  label: Spider Data API
  slug: spider-cloud-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-data-api-openapi.yml
- filename: spider-cloud-fetch-api-openapi.yml
  format: yaml
  label: Spider Fetch API
  slug: spider-cloud-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-fetch-api-openapi.yml
- filename: spider-cloud-links-api-openapi.yml
  format: yaml
  label: Spider Links API
  slug: spider-cloud-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-links-api-openapi.yml
- filename: spider-cloud-scraping-api-openapi.yml
  format: yaml
  label: Spider Scraping API
  slug: spider-cloud-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-scraping-api-openapi.yml
- filename: spider-cloud-screenshot-api-openapi.yml
  format: yaml
  label: Spider Screenshot API
  slug: spider-cloud-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-screenshot-api-openapi.yml
- filename: spider-cloud-search-api-openapi.yml
  format: yaml
  label: Spider Search API
  slug: spider-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-search-api-openapi.yml
- filename: spider-cloud-transform-api-openapi.yml
  format: yaml
  label: Spider Transform API
  slug: spider-cloud-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-transform-api-openapi.yml
- filename: spider-cloud-unblocker-api-openapi.yml
  format: yaml
  label: Spider Unblocker API
  slug: spider-cloud-unblocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-unblocker-api-openapi.yml
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
- Artificial Intelligence
- Markdown
- MCP
- Rust
- Headless Browser
- Proxies
---
