---
api_key_in: []
api_specs:
- filename: apify-api.yaml
  format: yaml
  label: Apify API
  slug: apify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apify
provider_slug: apify
scheme_count: 1
schemes:
- description: Bearer token from Apify console Settings > Integrations.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apify-api.yaml
  type: http
slug: apify-authentication
source_filename: apify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apify-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from Apify console Settings > Integrations.\n  sources:\n  - openapi/apify-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/authentication/apify-authentication.yml
summary_line: http · 1 scheme
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
---
