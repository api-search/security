---
anonymous_access: false
api_key_in:
- query
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Snap Api Website Screenshots In One Call Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snap API secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snap API
provider_slug: snap-api-website-screenshots-in-one-call
scheme_count: 3
schemes:
- aliases:
  - token
  - apiKey
  description: Pass the dashboard API key as the api_key query parameter (aliases token / apiKey accepted). Convenient for browser and n8n HTTP-node use; note it exposes the key in URLs and logs.
  in: query
  name: api_key_query
  parameter_name: api_key
  sources:
  - docs.html
  - llms.txt
  type: apiKey
- description: Pass the dashboard API key in the X-API-Key request header. Recommended for server-to-server use.
  in: header
  name: api_key_header
  parameter_name: X-API-Key
  sources:
  - docs.html
  - llms.txt
  type: apiKey
- description: 'Pass the dashboard API key as a bearer token via Authorization: Bearer <key>. Same key value as the other two methods.'
  name: bearer
  scheme: bearer
  sources:
  - docs.html
  - llms.txt
  type: http
slug: snap-api-website-screenshots-in-one-call-authentication
source_filename: snap-api-website-screenshots-in-one-call-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://snap.flyhold.in/docs.html\ndocs: https://snap.flyhold.in/docs.html\ncorroboration: >-\n  https://snap.flyhold.in/llms.txt states: Auth (any one) — query api_key, or header X-API-Key,\n  or Authorization Bearer <key>.\nchecked: '2026-09-17'\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  http_schemes: [bearer]\nnote: >-\n  Snap API uses a single opaque API key issued from the dashboard after signup (register.html grants\n  200 free credits). The same key may be presented three interchangeable ways. There is no OpenAPI\n  securityScheme published; this profile is read from the developer documentation and llms.txt, not\n  derived from a machine-readable contract.\nschemes:\n  - name: api_key_query\n    type: apiKey\n    in: query\n    parameter_name: api_key\n    aliases: [token, apiKey]\n    description: >-\n      Pass the dashboard API key as the api_key query parameter (aliases token / apiKey accepted).\n\
  \      Convenient for browser and n8n HTTP-node use; note it exposes the key in URLs and logs.\n    sources: [docs.html, llms.txt]\n  - name: api_key_header\n    type: apiKey\n    in: header\n    parameter_name: X-API-Key\n    description: Pass the dashboard API key in the X-API-Key request header. Recommended for server-to-server use.\n    sources: [docs.html, llms.txt]\n  - name: bearer\n    type: http\n    scheme: bearer\n    description: >-\n      Pass the dashboard API key as a bearer token via Authorization: Bearer <key>. Same key value\n      as the other two methods.\n    sources: [docs.html, llms.txt]\nfailure:\n  status: 403\n  meaning: Missing, invalid, or inactive API key.\nkey_provisioning:\n  signup_url: https://snap.flyhold.in/register.html\n  free_grant: 200 credits/month on the Developer tier\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap-api-website-screenshots-in-one-call/refs/heads/main/authentication/snap-api-website-screenshots-in-one-call-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- screenshot-api
- Developer Tools
- Web Capture
- n8n
- Web Scraping
- PDF Generation
- Automation
- Rendering
---
