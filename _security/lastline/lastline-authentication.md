---
api_key_in:
- query
- formData
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lastline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lastline secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lastline
provider_slug: lastline
scheme_count: 2
schemes:
- description: All Lastline Analyst API endpoints accept HTTP Basic Authentication, carrying the API key as the username and the API token as the password.
  name: HTTPBasic
  scheme: basic
  sources:
  - https://analysis.lastline.com/analysis/api-docs/html/api.html
  standard: RFC 7617
  type: http
- description: Credentials may be embedded directly in each request as the `key` and `api_token` parameter pair instead of using HTTP Basic. Both values are ASCII text and are only ever sent over HTTPS.
  in: request-parameter
  name: KeyAndToken
  parameters:
  - description: Lastline Analyst API key.
    name: key
    required: true
  - description: Secret Lastline Analyst API token.
    name: api_token
    required: true
  sources:
  - https://analysis.lastline.com/analysis/api-docs/html/api.html
  type: apiKey
slug: lastline-authentication
source_filename: lastline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://analysis.lastline.com/analysis/api-docs/html/api.html#authentication\ndocs: https://analysis.lastline.com/analysis/api-docs/html/api.html#authentication\nnote: >-\n  Captured from the live first-party Lastline Analyst API documentation (copyright 2009-2021 VMware,\n  Inc.), still served at analysis.lastline.com and user.lastline.com and verified HTTP 200 on\n  2026-07-19. No OpenAPI/Swagger definition was ever published, so this profile is transcribed from\n  the prose reference rather than derived from a spec.\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  - formData\n  oauth2_flows: []\n  session_based: true\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  standard: RFC 7617\n  description: All Lastline Analyst API endpoints accept HTTP Basic Authentication, carrying the API\n    key as the username and the API token as the password.\n  sources:\n  - https://analysis.lastline.com/analysis/api-docs/html/api.html\n\
  - name: KeyAndToken\n  type: apiKey\n  in: request-parameter\n  parameters:\n  - name: key\n    description: Lastline Analyst API key.\n    required: true\n  - name: api_token\n    description: Secret Lastline Analyst API token.\n    required: true\n  description: Credentials may be embedded directly in each request as the `key` and `api_token`\n    parameter pair instead of using HTTP Basic. Both values are ASCII text and are only ever sent\n    over HTTPS.\n  sources:\n  - https://analysis.lastline.com/analysis/api-docs/html/api.html\nsessions:\n  supported: true\n  login_operation: login\n  login_path: /analysis/login\n  ping_operation: ping\n  description: A client may call login() to validate credentials once and establish an HTTP session;\n    subsequent requests may present the session token instead of the credentials. ping() verifies an\n    active session.\n  expiry_error: ANALYSIS_API_AUTHENTICATION_REQUIRED\n  opt_out_header: x-nsx-lastline-no-session\n  opt_out_description:\
  \ >-\n    Setting `x-nsx-lastline-no-session: 1` mandates that the API not establish a session for the\n    request.\ncredential_issuance:\n  self_service: false\n  description: API key and API token were issued by Lastline (later VMware) to customers; there was\n    no public self-service signup for the Analyst API.\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastline/refs/heads/main/authentication/lastline-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Cybersecurity
- Malware Analysis
- Sandboxing
- Threat Intelligence
- Network Detection and Response
- Security
- Acquired
---
