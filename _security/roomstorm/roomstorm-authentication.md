---
api_key_in: []
auth_types:
- http
- cookie
description: ''
kind: authentication
layout: security
method: searched
name: Roomstorm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roomstorm secures its APIs with http and cookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Roomstorm
provider_slug: roomstorm
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JSON Web Token issued by POST /backend/v1/auth/ (username/password). Token carries a payload with username, user_id, email, orig_iat, exp; `expires` returned alongside. Present as an Authorization bearer header on protected endpoints.
  name: jwtAuth
  scheme: bearer
  sources:
  - api-blueprint/roomstorm-apiary.apib
  token_endpoint: https://www.roomstorm.com/backend/v1/auth/
  type: http
- description: Django session cookie set by the auth endpoint (httponly), paired with a csrftoken cookie for unsafe methods. Used by the first-party web/guest app.
  in: cookie
  name: sessionAuth
  parameter_name: sessionid
  sources:
  - api-blueprint/roomstorm-apiary.apib
  type: apiKey
slug: roomstorm-authentication
source_filename: roomstorm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://github.com/walksource/roomstorm-api (apiary.apib) + live behavior of\n  https://www.roomstorm.com/backend/v1/ (Django REST framework; 403 \"Authentication\n  credentials were not provided\" on protected collections)\nsummary:\n  types: [http, cookie]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    JWT bearer token obtained via username/password. POST /backend/v1/auth/ validates\n    credentials and returns a JWT (`token` + `expires` + `payload`) alongside a session\n    cookie (`sessionid`) and a CSRF cookie (`csrftoken`). Subsequent API calls\n    authenticate with either the JWT or the session cookie. No OAuth2 / API-key surface\n    is published. A separate guest/account web login lives at /backend/accounts/login/.\nschemes:\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    JSON Web Token issued by POST /backend/v1/auth/ (username/password). Token carries\n\
  \    a payload with username, user_id, email, orig_iat, exp; `expires` returned\n    alongside. Present as an Authorization bearer header on protected endpoints.\n  token_endpoint: https://www.roomstorm.com/backend/v1/auth/\n  sources: [api-blueprint/roomstorm-apiary.apib]\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter_name: sessionid\n  description: >-\n    Django session cookie set by the auth endpoint (httponly), paired with a csrftoken\n    cookie for unsafe methods. Used by the first-party web/guest app.\n  sources: [api-blueprint/roomstorm-apiary.apib]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roomstorm/refs/heads/main/authentication/roomstorm-authentication.yml
summary_line: http/cookie · 2 schemes
tags:
- Company
- Travel
- Hospitality
- Hotels
- Airlines
- Marketplace
- Bookings
- Y Combinator
---
