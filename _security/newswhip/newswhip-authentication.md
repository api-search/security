---
api_key_in:
- query
api_specs:
- filename: newswhip-openapi.yml
  format: yaml
  label: NewsWhip API
  slug: newswhip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Newswhip Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewsWhip secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NewsWhip
provider_slug: newswhip
scheme_count: 1
schemes:
- description: All requests are authenticated with a NewsWhip API key passed as the query parameter `key`. Keys are issued by NewsWhip on request (API access is provisioned per customer); there is no OAuth or self-service key generation.
  in: query
  name: sec0
  parameter: key
  sources:
  - openapi/newswhip-openapi.yml
  type: apiKey
slug: newswhip-authentication
source_filename: newswhip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/newswhip-openapi.yml\ndocs: https://developer.newswhip.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\nschemes:\n- name: sec0\n  type: apiKey\n  in: query\n  parameter: key\n  description: All requests are authenticated with a NewsWhip API key passed as the query parameter `key`.\n    Keys are issued by NewsWhip on request (API access is provisioned per customer); there is no OAuth\n    or self-service key generation.\n  sources:\n  - openapi/newswhip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/authentication/newswhip-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Media Intelligence
- Social Media Analytics
- News
- Content Analytics
- Engagement Data
- Predictive Analytics
- Media Monitoring
---
