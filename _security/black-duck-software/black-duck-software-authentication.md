---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Black Duck Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Black Duck Software secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Black Duck Software
provider_slug: black-duck-software
scheme_count: 2
schemes:
- description: 'A user generates a long-lived API token in the Black Duck UI (My Access Tokens). The token is exchanged for a short-lived bearer token by POSTing to /api/tokens/authenticate with an "Authorization: token <API_TOKEN>" header.

    '
  in: header
  name: ApiToken
  parameter: Authorization
  sources:
  - https://documentation.blackduck.com/category/api
  type: apiKey
- description: 'Authenticated API calls pass the short-lived bearer token (returned by the authenticate call) as "Authorization: Bearer <token>". Tokens expire and must be refreshed.

    '
  name: BearerAuth
  scheme: bearer
  sources:
  - https://documentation.blackduck.com/category/api
  type: http
slug: black-duck-software-authentication
source_filename: black-duck-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://documentation.blackduck.com/category/api\ndocs: https://documentation.blackduck.com/bundle/bd-hub/page/SDK/Using_the_Hub_SDK.html\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: []\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >\n    A user generates a long-lived API token in the Black Duck UI (My Access Tokens). The token is\n    exchanged for a short-lived bearer token by POSTing to /api/tokens/authenticate with an\n    \"Authorization: token <API_TOKEN>\" header.\n  sources: [https://documentation.blackduck.com/category/api]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >\n    Authenticated API calls pass the short-lived bearer token (returned by the authenticate call)\n    as \"Authorization: Bearer <token>\". Tokens expire and must be refreshed.\n  sources: [https://documentation.blackduck.com/category/api]\n\
  notes: >\n  The Black Duck Hub REST API is per-tenant (each customer runs its own hub instance), so there is\n  no single public base URL. Auth is token-based: an API token minted in the UI is authenticated to\n  obtain a time-limited bearer token used on subsequent calls. Requests also require Black Duck's\n  custom versioned media types in Accept/Content-Type headers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-duck-software/refs/heads/main/authentication/black-duck-software-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Security
- Application Security
- Software Composition Analysis
- Open Source Security
- Static Analysis
- DevSecOps
- Vulnerability Management
- SAST
- SCA
---
