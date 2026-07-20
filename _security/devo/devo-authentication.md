---
api_key_in:
- header
auth_types:
- apiKey-hmac
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Devo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Devo secures its APIs with apiKey-hmac and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Devo
provider_slug: devo
scheme_count: 2
schemes:
- description: Sign each request with the domain API key and secret. The signature is HMAC-SHA256 over the request body/data plus the API key and timestamp, sent hex-encoded.
  headers:
  - name: x-logtrust-apikey
    value: <domain API key>
  - name: x-logtrust-timestamp
    value: <request timestamp in ms>
  - name: x-logtrust-sign
    value: <HMAC-SHA256(apikey + data + timestamp, apiSecret) hex>
  in: header
  name: HMAC signed request
  sources:
  - https://github.com/DevoInc/python-sdk/blob/master/devo/api/client.py
  type: apiKey
- description: Authenticate with a standalone access token generated in the Devo web UI. Sent as an Authorization Bearer header alongside a request timestamp.
  headers:
  - name: Authorization
    value: Bearer <standalone token>
  - name: x-logtrust-timestamp
    value: <request timestamp in ms>
  name: Standalone Bearer token
  scheme: bearer
  sources:
  - https://github.com/DevoInc/python-sdk/blob/master/devo/api/client.py
  type: http
slug: devo-authentication
source_filename: devo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docs.devo.com/space/latest/95128251/API+reference (Authorizing REST API\n  requests) and the first-party python-sdk client\n  (https://github.com/DevoInc/python-sdk/blob/master/devo/api/client.py)\ndocs: https://docs.devo.com/confluence/ndt/api-reference/rest-api/authorizing-rest-api-requests\nsummary:\n  types: [apiKey-hmac, http-bearer]\n  api_key_in: [header]\n  notes: >-\n    Devo REST API requests authenticate with domain-scoped credentials created in\n    Administration -> Credentials -> Access Keys. Two schemes are supported: (1)\n    an API key + API secret used to HMAC-SHA256-sign each request, or (2) a\n    standalone Bearer token. Credentials are domain- and region-scoped.\nschemes:\n- name: HMAC signed request\n  type: apiKey\n  in: header\n  description: >-\n    Sign each request with the domain API key and secret. The signature is\n    HMAC-SHA256 over the request body/data plus the API key and timestamp,\
  \ sent\n    hex-encoded.\n  headers:\n  - name: x-logtrust-apikey\n    value: \"<domain API key>\"\n  - name: x-logtrust-timestamp\n    value: \"<request timestamp in ms>\"\n  - name: x-logtrust-sign\n    value: \"<HMAC-SHA256(apikey + data + timestamp, apiSecret) hex>\"\n  sources:\n  - https://github.com/DevoInc/python-sdk/blob/master/devo/api/client.py\n- name: Standalone Bearer token\n  type: http\n  scheme: bearer\n  description: >-\n    Authenticate with a standalone access token generated in the Devo web UI.\n    Sent as an Authorization Bearer header alongside a request timestamp.\n  headers:\n  - name: Authorization\n    value: \"Bearer <standalone token>\"\n  - name: x-logtrust-timestamp\n    value: \"<request timestamp in ms>\"\n  sources:\n  - https://github.com/DevoInc/python-sdk/blob/master/devo/api/client.py\ndata_ingestion:\n  note: >-\n    Event ingestion (sending data to Devo) is authenticated separately using\n    mutual-TLS X.509 domain certificates (key + cert + CA\
  \ chain) over the secure\n    sending endpoints, distinct from the REST API key/token schemes above.\n  sources:\n  - https://docs.devo.com/space/latest/94658823/Sending+data+to+the+HTTP+API+endpoint\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devo/refs/heads/main/authentication/devo-authentication.yml
summary_line: apiKey-hmac/http-bearer · 2 schemes
tags:
- Company
- Cybersecurity
- SIEM
- Security
- Security Data Platform
- Threat Detection
- Log Management
- Analytics
- Observability
- Query API
---
