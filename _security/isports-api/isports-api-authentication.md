---
api_key_in:
- query
api_specs:
- filename: isports-api-basketball-common-api-api-openapi.yml
  format: yaml
  label: iSports API Basketball Common API API
  slug: isports-api-basketball-common-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-common-api-api-openapi.yml
- filename: isports-api-basketball-live-animation-api-openapi.yml
  format: yaml
  label: iSports API Basketball Live animation API
  slug: isports-api-basketball-live-animation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-live-animation-api-openapi.yml
- filename: isports-api-basketball-live-data-api-openapi.yml
  format: yaml
  label: iSports API Basketball Live Data API
  slug: isports-api-basketball-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-live-data-api-openapi.yml
- filename: isports-api-basketball-odds-api-openapi.yml
  format: yaml
  label: iSports API Basketball Odds API
  slug: isports-api-basketball-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-odds-api-openapi.yml
- filename: isports-api-basketball-profile-api-openapi.yml
  format: yaml
  label: iSports API Basketball Profile API
  slug: isports-api-basketball-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-profile-api-openapi.yml
- filename: isports-api-basketball-stats-api-openapi.yml
  format: yaml
  label: iSports API Basketball Stats API
  slug: isports-api-basketball-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-basketball-stats-api-openapi.yml
- filename: isports-api-football-common-api-api-openapi.yml
  format: yaml
  label: iSports API Football Common API API
  slug: isports-api-football-common-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-common-api-api-openapi.yml
- filename: isports-api-football-european-odds-200-agencies-api-openapi.yml
  format: yaml
  label: iSports API Football European Odds (200+ Agencies) API
  slug: isports-api-football-european-odds-200-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-european-odds-200-agencies-api-openapi.yml
- filename: isports-api-football-live-animation-api-openapi.yml
  format: yaml
  label: iSports API Football Live animation API
  slug: isports-api-football-live-animation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-live-animation-api-openapi.yml
- filename: isports-api-football-live-data-api-openapi.yml
  format: yaml
  label: iSports API Football Live Data API
  slug: isports-api-football-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-live-data-api-openapi.yml
- filename: isports-api-football-multiple-languages-api-openapi.yml
  format: yaml
  label: iSports API Football Multiple languages API
  slug: isports-api-football-multiple-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-multiple-languages-api-openapi.yml
- filename: isports-api-football-odds-18-agencies-api-openapi.yml
  format: yaml
  label: iSports API Football Odds (18 Agencies) API
  slug: isports-api-football-odds-18-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-odds-18-agencies-api-openapi.yml
- filename: isports-api-football-other-odds-api-openapi.yml
  format: yaml
  label: iSports API Football Other Odds API
  slug: isports-api-football-other-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-other-odds-api-openapi.yml
- filename: isports-api-football-profile-api-openapi.yml
  format: yaml
  label: iSports API Football Profile API
  slug: isports-api-football-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-profile-api-openapi.yml
- filename: isports-api-football-stats-api-openapi.yml
  format: yaml
  label: iSports API Football Stats API
  slug: isports-api-football-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/openapi/isports-api-football-stats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Isports Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: iSports API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iSports API
provider_slug: isports-api
scheme_count: 1
schemes:
- description: Personal API key issued automatically when an account is created and shown in the account settings page. It is passed on every request as the `api_key` query parameter — there is no header form, no bearer token, no OAuth, and no signing.
  docs: https://www.isportsapi.com/en/docs.html?id=news_0
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/isports-api-openapi.yml
  type: apiKey
slug: isports-api-authentication
source_filename: isports-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/isports-api-openapi.yml\ndocs: https://www.isportsapi.com/en/docs.html?id=news_0\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    Personal API key issued automatically when an account is created and shown in the account settings page.\n    It is passed on every request as the `api_key` query parameter — there is no header form, no bearer token,\n    no OAuth, and no signing.\n  sources:\n  - openapi/isports-api-openapi.yml\n  docs: https://www.isportsapi.com/en/docs.html?id=news_0\nkey_lifecycle:\n  issued_at: account creation (one key per account)\n  console: https://www.isportsapi.com/en/user/accountSettings\n  rotation_documented: false\n  expiry: >-\n    The key deactivates when the free trial or subscription lapses; calls then return the standard envelope with\n    a non-zero `code`.\n  entitlement:\
  \ >-\n    A single key is scoped by the products the account has subscribed to. Calling an endpoint outside the\n    subscribed plan fails the same way an invalid key does.\nobservations:\n- >-\n  The key travels in the query string, so it is written to server access logs, browser history, and any\n  intermediary proxy log. There is no header alternative documented.\n- >-\n  Authentication failure returns HTTP 200 with `{\"code\":2,\"message\":\"Invalid [api_key], illegal access.\"}` —\n  not 401. Verified live 2026-08-09 against https://api.isportsapi.com/sport/football/livescores.\n- >-\n  The documentation shows both `http://` and `https://` request forms. HTTPS is live on both hosts (TLS 1.2,\n  verified 2026-08-09) but no HSTS is served, so a plaintext http:// call carrying the key will go through.\n- >-\n  The embeddable widget/animation products use a different credential entirely — an `accessKey` plus a domain\n  whitelist. See components/isports-api-components.yml.\nx-evidence:\n\
  \  fetched: '2026-08-09'\n  url: https://api.isportsapi.com/sport/football/livescores\n  http_status: 200\n  body: '{\"code\":2,\"message\":\"Invalid [api_key], illegal access.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isports-api/refs/heads/main/authentication/isports-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports API
- Sports Data
- Football
- Basketball
- Odds
- Live Data
- Sports Statistics
- Live Scores
- Widgets
- REST API
---
