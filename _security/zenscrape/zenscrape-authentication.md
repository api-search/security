---
api_key_in:
- header
api_specs:
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Scrape API
  slug: zenscrape-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Account API
  slug: zenscrape-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zenscrape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenscrape secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zenscrape
provider_slug: zenscrape
scheme_count: 1
schemes:
- description: API key issued from the Zenscrape dashboard. May also be supplied as the `apikey` query parameter or form field.
  in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/zenscrape-openapi.yml
  type: apiKey
slug: zenscrape-authentication
source_filename: zenscrape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenscrape-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key issued from the Zenscrape dashboard. May also be supplied as the `apikey`\n    query parameter or form field.\n  sources:\n  - openapi/zenscrape-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/authentication/zenscrape-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Scraping
- Proxy
- HTML
- Data Extraction
- JavaScript Rendering
---
