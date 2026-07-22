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
name: Truevault Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueVault secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TrueVault
provider_slug: truevault
scheme_count: 2
schemes:
- description: A user's API_KEY is issued at user creation via the Management Console or the Users API and does not expire unless explicitly expired. It is placed as the Basic-auth username (colon appended, Base64-encoded). Recommended for administrators, owners, and developers.
  in: header
  name: apiKey
  scheme: basic
  source: https://docs.truevault.com/Overview.html
  type: apiKey
- description: A user ACCESS_TOKEN is issued via the Users API or the /auth/login endpoint (default 24-hour expiry, overridable with not_valid_after). Supplied as the Basic-auth username. Recommended for regular end-users.
  name: accessToken
  scheme: basic
  source: https://docs.truevault.com/Overview.html
  type: http
slug: truevault-authentication
source_filename: truevault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.truevault.com/Overview.html\ndocs: https://docs.truevault.com/Overview.html\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [basic]\n  oauth2_flows: []\n  notes: >-\n    TrueVault Safe authenticates with either a long-lived API key or a\n    short-lived user access token. Both are supplied as the username in an HTTP\n    Basic Authorization header (the password is left empty and the\n    \"<credential>:\" string is Base64-encoded). There is no OAuth 2.0 / OIDC\n    surface; fine-grained authorization is handled by Group policies (the Access\n    Grid), not OAuth scopes.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  scheme: basic\n  description: >-\n    A user's API_KEY is issued at user creation via the Management Console or\n    the Users API and does not expire unless explicitly expired. It is placed as\n    the Basic-auth username (colon appended, Base64-encoded). Recommended\
  \ for\n    administrators, owners, and developers.\n  source: https://docs.truevault.com/Overview.html\n- name: accessToken\n  type: http\n  scheme: basic\n  description: >-\n    A user ACCESS_TOKEN is issued via the Users API or the /auth/login endpoint\n    (default 24-hour expiry, overridable with not_valid_after). Supplied as the\n    Basic-auth username. Recommended for regular end-users.\n  source: https://docs.truevault.com/Overview.html\nauthorization:\n  model: group-policy\n  description: >-\n    Authorization is enforced by Group policies over an Access Grid: activities\n    (Create/Read/Update/Delete/etc.) are granted per resource type and per\n    resource id to the groups a user belongs to.\n  docs: https://docs.truevault.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truevault/refs/heads/main/authentication/truevault-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Data Privacy
- Security
- Compliance
- HIPAA
- Data Storage
- Encryption
- Identity
- Privacy
- PII
---
