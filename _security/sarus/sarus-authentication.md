---
anonymous_access: true
api_key_in: []
auth_types:
- session-cookie
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sarus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sarus secures its APIs with session-cookie and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sarus
provider_slug: sarus
scheme_count: 3
schemes:
- applies_to: sarus:sarus-gateway
  failure: HTTP 401 on incorrect credentials
  login_request: POST {gateway}/login with JSON body {"email", "password"}
  name: credentialsLogin
  note: The client requires the base URL to end with /gateway (Client._URL_SUFFIX).
  session: the requests.Session keeps the cookie the Gateway sets and replays it on every call
  type: session-cookie
- applies_to: sarus:sarus-gateway
  login_request: browser opens GET {gateway}/oidc_login?headless=true
  name: googleOidcLogin
  provider: Google
  sdk_option: Client(url=..., google_login=True)
  session: the user pastes a base64 token from the login page; the client decodes it and sets it as the 'session' cookie
  type: openIdConnect
- applies_to: sarus:qrlew-server
  name: none
  note: The Qrlew server README and published request examples carry no credentials or auth headers. Its GET /public_key and POST /verify endpoints concern signing of rewritten queries, not caller authentication.
  type: none
slug: sarus-authentication
source_filename: sarus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://files.pythonhosted.org/packages/45/e3/3cb946afbd3e32f30a43cbe68a1c6e7d8a32b4873664a3c4ba5a180f0e67/sarus-0.12.0.tar.gz\nsource_file: sarus-0.12.0/sarus/sarus.py (class Client)\nnote: >-\n  Sarus publishes no OpenAPI and its reference at docs.sarus.tech is access-controlled, so this\n  profile is read from the first-party 'sarus' Python client (PyPI 0.12.0, published by Sarus\n  Technologies) — the code that actually authenticates against a Sarus Gateway. It applies to the\n  customer-deployed Sarus Gateway only. The open-source Qrlew server (github.com/Qrlew/server)\n  documents no authentication at all.\nsummary:\n  types: [session-cookie, openIdConnect]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: credentialsLogin\n  type: session-cookie\n  applies_to: sarus:sarus-gateway\n  login_request: POST {gateway}/login with JSON body {\"email\", \"password\"}\n  session: the requests.Session keeps the cookie the\
  \ Gateway sets and replays it on every call\n  failure: HTTP 401 on incorrect credentials\n  note: The client requires the base URL to end with /gateway (Client._URL_SUFFIX).\n- name: googleOidcLogin\n  type: openIdConnect\n  applies_to: sarus:sarus-gateway\n  provider: Google\n  login_request: browser opens GET {gateway}/oidc_login?headless=true\n  session: >-\n    the user pastes a base64 token from the login page; the client decodes it and sets it as the\n    'session' cookie\n  sdk_option: Client(url=..., google_login=True)\n- name: none\n  type: none\n  applies_to: sarus:qrlew-server\n  note: >-\n    The Qrlew server README and published request examples carry no credentials or auth headers.\n    Its GET /public_key and POST /verify endpoints concern signing of rewritten queries, not\n    caller authentication.\nheaders:\n- name: SARUS-Client-SDK-Version\n  sent_by: sarus Python client on every request\n  value: the installed client version\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarus/refs/heads/main/authentication/sarus-authentication.yml
summary_line: session-cookie/openIdConnect · 3 schemes
tags:
- Company
- Ai Data
- Privacy
- Differential Privacy
- Synthetic Data
- Analytics
- Machine-Learning
- Data Governance
- SQL
- Open-Source
---
