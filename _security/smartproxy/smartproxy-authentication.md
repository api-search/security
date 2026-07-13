---
api_key_in:
- header
api_specs:
- filename: smartproxy-openapi.yml
  format: yaml
  label: Smartproxy Account Management API
  slug: proxy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartproxy/refs/heads/main/openapi/smartproxy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartproxy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartproxy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartproxy
provider_slug: smartproxy
scheme_count: 1
schemes:
- description: API key obtained via the /auth endpoint
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/smartproxy-openapi.yml
  type: apiKey
slug: smartproxy-authentication
source_filename: smartproxy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartproxy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key obtained via the /auth endpoint\n  sources:\n  - openapi/smartproxy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartproxy/refs/heads/main/authentication/smartproxy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Proxies
- Web Scraping
- Data Collection
- Residential Proxies
- Datacenter Proxies
- Mobile Proxies
- Network Infrastructure
---
