---
api_key_in: []
api_specs:
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Web Scraper API
  slug: oxylabs-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Residential Public API
  slug: oxylabs-residential-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Dashboard API
  slug: oxylabs-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oxylabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oxylabs secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oxylabs
provider_slug: oxylabs
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/oxylabs-openapi.yml
  type: http
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oxylabs-openapi.yml
  type: http
slug: oxylabs-authentication
source_filename: oxylabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oxylabs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/oxylabs-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/oxylabs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/authentication/oxylabs-authentication.yml
summary_line: http · 2 schemes
tags:
- AI Web Scraping
- Bot Mitigation Bypass
- CAPTCHA Solving
- Data Extraction
- Datacenter Proxies
- Datasets
- E-Commerce Data
- Headless Browser
- ISP Proxies
- Mobile Proxies
- Proxies
- Residential Proxies
- SERP
- Scraper API
- Scraping
- Web Data
- Web Intelligence
- Web Unblocker
---
