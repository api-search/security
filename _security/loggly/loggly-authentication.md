---
api_key_in:
- query
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Loggly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loggly secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loggly
provider_slug: loggly
scheme_count: 3
schemes:
- applies_to: Loggly Event Retrieval API (apiv2)
  docs: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/token-based-api-authentication.htm
  format: 'Authorization: bearer <api-token>'
  location: Authorization header
  name: apiToken
  provisioning: Created in Loggly Log Settings > API Tokens > Add New. Used for search, events, iterate, fields, and stats endpoints.
  scheme: bearer
  type: http
- applies_to: Loggly HTTP/S Event Endpoint (ingestion)
  docs: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/http-endpoint.htm
  format: https://logs-01.loggly.com/inputs/<customer-token>/tag/<tags>/
  in: path
  name: customerToken
  name_hint: token
  provisioning: Found under Loggly Source Setup > Customer Tokens; embedded in the ingestion URL path. Sends log data only; rejected by the retrieval API.
  type: apiKey
- applies_to: Loggly Event Retrieval API (apiv2) — legacy
  format: account username:password
  name: basicAuth
  note: Legacy alternative to bearer API token for retrieval API calls.
  scheme: basic
  type: http
slug: loggly-authentication
source_filename: loggly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/token-based-api-authentication.htm\ndocs: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/token-based-api-authentication.htm\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  api_key_in: [query]\n  note: >-\n    Two distinct token classes. API tokens authenticate the event-retrieval REST\n    API (apiv2) and MUST NOT be used to send data. Customer tokens authenticate\n    the HTTP/S ingestion endpoint and must NOT be used to query. Basic auth with\n    Loggly account username/password is also historically supported for the\n    retrieval API but bearer API tokens are the current recommendation.\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  applies_to: Loggly Event Retrieval API (apiv2)\n  location: Authorization header\n  format: 'Authorization: bearer <api-token>'\n  provisioning: >-\n    Created\
  \ in Loggly Log Settings > API Tokens > Add New. Used for search,\n    events, iterate, fields, and stats endpoints.\n  docs: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/token-based-api-authentication.htm\n- name: customerToken\n  type: apiKey\n  in: path\n  name_hint: token\n  applies_to: Loggly HTTP/S Event Endpoint (ingestion)\n  format: 'https://logs-01.loggly.com/inputs/<customer-token>/tag/<tags>/'\n  provisioning: >-\n    Found under Loggly Source Setup > Customer Tokens; embedded in the ingestion\n    URL path. Sends log data only; rejected by the retrieval API.\n  docs: https://documentation.solarwinds.com/en/success_center/loggly/content/admin/http-endpoint.htm\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: Loggly Event Retrieval API (apiv2) — legacy\n  format: 'account username:password'\n  note: Legacy alternative to bearer API token for retrieval API calls.\nmfa:\n  available: true\n  note: >-\n    Multi-Factor Authentication\
  \ (2FA) is available for SolarWinds Application\n    Management / Loggly user accounts protecting the console (not API calls).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loggly/refs/heads/main/authentication/loggly-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Developer Tools
- Logging
- Log Management
- Observability
- Monitoring
- DevOps
- Analytics
- SaaS
---
