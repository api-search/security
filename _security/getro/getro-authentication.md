---
api_key_in: []
auth_types:
- http
description: The Getro Network API (v2) authenticates every request with a static API key presented as an HTTP Bearer token. API keys are generated in the Getro admin portal (getro.com/app, now hosted at getro.findem.ai) and a developer key can be requested from help@getro.com. There is no OAuth, no OpenID Connect, and no per-scope authorization surface — a single account-scoped key grants access to that account's networks, companies, jobs and contacts. Browser (CORS) requests are explicitly not supported; the key must be used server-side.
kind: authentication
layout: security
method: searched
name: Getro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Getro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Getro
provider_slug: getro
scheme_count: 1
schemes:
- description: 'Send the API key in the Authorization header as `Authorization: Bearer API_KEY`. Keys are account-scoped and issued from the Getro admin portal.'
  format: Bearer <API_KEY>
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  sources:
  - https://developers.getro.com/
  type: http
slug: getro-authentication
source_filename: getro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.getro.com/\ndocs: https://developers.getro.com/\ndescription: >-\n  The Getro Network API (v2) authenticates every request with a static API key\n  presented as an HTTP Bearer token. API keys are generated in the Getro admin\n  portal (getro.com/app, now hosted at getro.findem.ai) and a developer key can\n  be requested from help@getro.com. There is no OAuth, no OpenID Connect, and no\n  per-scope authorization surface — a single account-scoped key grants access to\n  that account's networks, companies, jobs and contacts. Browser (CORS) requests\n  are explicitly not supported; the key must be used server-side.\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Send the API key in the Authorization header as `Authorization: Bearer API_KEY`.\n    Keys are account-scoped and issued\
  \ from the Getro admin portal.\n  in: header\n  header: Authorization\n  format: 'Bearer <API_KEY>'\n  sources:\n  - https://developers.getro.com/\nnotes:\n  - Rate limited to 30 requests per minute (see rate-limits/getro-rate-limits.yml).\n  - CORS is not supported; requests must originate server-side.\n  - Request a developer key via help@getro.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getro/refs/heads/main/authentication/getro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Jobs
- Talent
- Hiring
- Recruiting
- Job Board
- Venture Capital
- Networks
- CRM
---
