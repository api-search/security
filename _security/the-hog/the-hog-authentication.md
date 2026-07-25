---
api_key_in:
- header
api_specs:
- filename: the-hog-company-search-api-openapi.yml
  format: yaml
  label: The Hog Company Search API
  slug: the-hog-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-company-search-api-openapi.yml
- filename: the-hog-deep-research-api-openapi.yml
  format: yaml
  label: The Hog Deep Research API
  slug: the-hog-deep-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-deep-research-api-openapi.yml
- filename: the-hog-enrichments-api-openapi.yml
  format: yaml
  label: The Hog Enrichments API
  slug: the-hog-enrichments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-enrichments-api-openapi.yml
- filename: the-hog-monitors-api-openapi.yml
  format: yaml
  label: The Hog Monitors API
  slug: the-hog-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-monitors-api-openapi.yml
- filename: the-hog-operations-api-openapi.yml
  format: yaml
  label: The Hog Operations API
  slug: the-hog-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-operations-api-openapi.yml
- filename: the-hog-people-search-api-openapi.yml
  format: yaml
  label: The Hog People Search API
  slug: the-hog-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-people-search-api-openapi.yml
- filename: the-hog-scrapers-api-openapi.yml
  format: yaml
  label: The Hog Scrapers API
  slug: the-hog-scrapers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-scrapers-api-openapi.yml
- filename: the-hog-search-api-openapi.yml
  format: yaml
  label: The Hog Search API
  slug: the-hog-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Hog Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Hog secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: The Hog
provider_slug: the-hog
scheme_count: 2
schemes:
- description: The public API key from the Credentials page.
  in: header
  name: AccessKey
  parameter: X-Access-Key
  sources:
  - openapi/the-hog-openapi.json
  type: apiKey
- description: The API secret shown when the credential is created.
  in: header
  name: SecretKey
  parameter: X-Secret-Key
  sources:
  - openapi/the-hog-openapi.json
  type: apiKey
slug: the-hog-authentication
source_filename: the-hog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/the-hog-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: header\n  parameter: X-Access-Key\n  description: The public API key from the Credentials page.\n  sources:\n  - openapi/the-hog-openapi.json\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: X-Secret-Key\n  description: The API secret shown when the credential is created.\n  sources:\n  - openapi/the-hog-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/authentication/the-hog-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- GTM Intelligence
- Sales Intelligence
- Data Enrichment
- Web Scraping
- People Data
- Company Data
- Deep Research
- Social Monitoring
- MCP
- AI Agents
- Y Combinator
---
