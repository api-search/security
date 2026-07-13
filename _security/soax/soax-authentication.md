---
api_key_in:
- header
api_specs:
- filename: soax-web-data-api-openapi.yml
  format: yaml
  label: SOAX Web Data API
  slug: soax-web-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/openapi/soax-web-data-api-openapi.yml
- filename: soax-proxy-management-api-openapi.yml
  format: yaml
  label: SOAX Proxy Management API
  slug: soax-proxy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/openapi/soax-proxy-management-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Soax Authentication
name_suffix: Authentication
oauth_flows: []
overview: SOAX secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SOAX
provider_slug: soax
scheme_count: 2
schemes:
- description: Your SOAX API key from the Profile tab in your dashboard
  in: header
  name: APIKeyHeader
  parameter: api-key
  sources:
  - openapi/soax-proxy-management-api-openapi.yml
  type: apiKey
- description: SOAX API key from your dashboard Scraper APIs section
  in: header
  name: APIKeyHeader
  parameter: X-SOAX-API-Secret
  sources:
  - openapi/soax-web-data-api-openapi.yml
  type: apiKey
slug: soax-authentication
source_filename: soax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soax-proxy-management-api-openapi.yml, openapi/soax-web-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Your SOAX API key from the Profile tab in your dashboard\n  sources:\n  - openapi/soax-proxy-management-api-openapi.yml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-SOAX-API-Secret\n  description: SOAX API key from your dashboard Scraper APIs section\n  sources:\n  - openapi/soax-web-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/authentication/soax-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Proxy
- Web Scraping
- Residential Proxies
- Mobile Proxies
- Datacenter Proxies
- Data Extraction
- Anti-Bot Bypass
---
