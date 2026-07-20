---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hackerrank Authentication
name_suffix: Authentication
oauth_flows: []
overview: HackerRank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HackerRank
provider_slug: hackerrank
scheme_count: 1
schemes:
- description: 'Per-account API key sent as an Authorization Bearer token. Generated in the HackerRank for Work account settings and passed as `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://www.hackerrank.com/work/apidocs
  type: http
slug: hackerrank-authentication
source_filename: hackerrank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.hackerrank.com/work/apidocs\nnotes: >-\n  No OpenAPI is published, so this profile is derived from the public HackerRank for Work API\n  documentation and a live probe. GET https://www.hackerrank.com/x/api/v3/tests returns HTTP 401\n  Unauthorized without credentials, confirming the API is token-gated. HackerRank for Work issues a\n  per-account API key (generated in account settings) that is sent as an HTTP Bearer token.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Per-account API key sent as an Authorization Bearer token. Generated in the HackerRank for Work\n    account settings and passed as `Authorization: Bearer <API_KEY>`.\n  sources:\n  - https://www.hackerrank.com/work/apidocs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackerrank/refs/heads/main/authentication/hackerrank-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Skills
- Technical Hiring
- Coding Assessment
- Recruiting
- Interviewing
- Education
- Developer Tools
---
