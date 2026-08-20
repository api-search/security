---
api_key_in:
- cookie
- header
api_specs:
- filename: xquik-rest-api-openapi.yml
  format: yaml
  label: Xquik REST API
  slug: xquik-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/openapi/xquik-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xquik Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xquik secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xquik
provider_slug: xquik-api
scheme_count: 3
schemes:
- description: 'Xquik API key passed through the x-api-key header. Xquik-Api-Key is a vendor-prefixed alias. API keys beginning with xq_ can also use Authorization: Bearer.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/xquik-rest-api-openapi.yml
  type: apiKey
- description: 'OAuth 2.1 access token passed through Authorization: Bearer. Values beginning with xq_ remain Xquik API-key credentials, not OAuth tokens.'
  name: oauthBearer
  scheme: bearer
  sources:
  - openapi/xquik-rest-api-openapi.yml
  type: http
- description: Secure Xquik browser session cookie.
  in: cookie
  name: cookieSession
  parameter: __Host-xquik_session
  sources:
  - openapi/xquik-rest-api-openapi.yml
  type: apiKey
slug: xquik-api-authentication
source_filename: xquik-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/xquik-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Xquik API key passed through the x-api-key header. Xquik-Api-Key is a vendor-prefixed\n    alias. API keys beginning with xq_ can also use Authorization: Bearer.'\n  sources:\n  - openapi/xquik-rest-api-openapi.yml\n- name: oauthBearer\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.1 access token passed through Authorization: Bearer. Values beginning\n    with xq_ remain Xquik API-key credentials, not OAuth tokens.'\n  sources:\n  - openapi/xquik-rest-api-openapi.yml\n- name: cookieSession\n  type: apiKey\n  in: cookie\n  parameter: __Host-xquik_session\n  description: Secure Xquik browser session cookie.\n  sources:\n  - openapi/xquik-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/authentication/xquik-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- social-media-data
- X / Twitter
- Social Listening
- Data Extraction
- Automation
- Webhook
- MCP
- Developer API
---
