---
api_key_in:
- header
api_specs:
- filename: the-hog-openapi.json
  format: json
  label: The Hog API
  slug: the-hog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-hog/refs/heads/main/openapi/the-hog-openapi.json
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
