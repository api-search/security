---
api_key_in: []
auth_types:
- http
- oauth1
description: ''
kind: authentication
layout: security
method: searched
name: Basekit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basekit secures its APIs with http and oauth1 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Basekit
provider_slug: basekit
scheme_count: 2
schemes:
- description: HTTP Basic Auth with username and password credentials scoped to a brand.
  name: basicAuth
  recommended: true
  scheme: basic
  source: https://apidocs.basekit.com/api/overview/
  type: http
- description: OAuth 1.0 is supported as an alternative to Basic Auth.
  name: oauth1
  source: https://apidocs.basekit.com/api/overview/
  type: oauth1
slug: basekit-authentication
source_filename: basekit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://apidocs.basekit.com/api/overview/\ndocs: https://apidocs.basekit.com/api/overview/\nsummary:\n  types:\n  - http\n  - oauth1\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The BaseKit REST API recommends HTTP Basic authentication (username/password) for its\n    relative simplicity, and also supports OAuth 1.0. Requests must send a valid User-Agent\n    header; POST/PUT bodies are JSON (Content-Type application/json).\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  recommended: true\n  description: HTTP Basic Auth with username and password credentials scoped to a brand.\n  source: https://apidocs.basekit.com/api/overview/\n- name: oauth1\n  type: oauth1\n  description: OAuth 1.0 is supported as an alternative to Basic Auth.\n  source: https://apidocs.basekit.com/api/overview/\nwebhook_auth:\n  scheme: hmac-sha256\n  header: X-Delivery-Hmac-SHA256\n  description: >-\n    Outgoing webhooks carry\
  \ an HMAC-SHA256 signature in the X-Delivery-Hmac-SHA256 header,\n    computed with a per-consumer HMAC secret, which the consumer can optionally validate.\n  source: https://apidocs.basekit.com/webhooks/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basekit/refs/heads/main/authentication/basekit-authentication.yml
summary_line: http/oauth1 · 2 schemes
tags:
- Company
- Website Builder
- Web Hosting
- E-Commerce
- White Label
- SaaS
- Small Business
- Website Migration
- Reseller
---
