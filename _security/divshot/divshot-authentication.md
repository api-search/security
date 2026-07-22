---
api_key_in: []
auth_types:
- http
- oauth2-like
description: ''
kind: authentication
layout: security
method: searched
name: Divshot Authentication
name_suffix: Authentication
oauth_flows:
- password
- github-browser-popup
overview: Divshot secures its APIs with http and oauth2-like across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and github-browser-popup flow(s).
provider_name: Divshot
provider_slug: divshot
scheme_count: 3
schemes:
- description: Long-lived Divshot access token passed to the client (`token` option) or to the CLI via `-t, --token`. Obtainable from the CLI with `auth:token`.
  name: accessToken
  scheme: bearer
  sources:
  - https://github.com/divshot/divshot-api/blob/master/README.md
  - https://github.com/divshot/divshot-cli/blob/master/README.md
  type: http
- description: Email + password exchanged for an access token via `divshot.auth('password', {email, password})`. The docs state passwords MUST NOT be stored and should only come from direct user input.
  flow: password
  name: passwordGrant
  requires_client_id: true
  sources:
  - https://github.com/divshot/divshot-api/blob/master/README.md
  type: oauth2
- description: Popup-based browser authentication, `divshot.auth('github')`, returning a user object and an access_token without the integrator handling credentials.
  flow: browser-popup
  name: githubBrowserAuth
  requires_client_id: true
  sources:
  - https://github.com/divshot/divshot-api/blob/master/README.md
  type: oauth2
slug: divshot-authentication
source_filename: divshot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/divshot/divshot-api/blob/master/README.md\ndocs: https://github.com/divshot/divshot-api#instantiate\nstatus: abandoned\nnotes: >-\n  Derived from the first-party divshot-api client README, the only surviving\n  public description of the Divshot API's authentication model. No OpenAPI was\n  ever published and api.divshot.com no longer resolves, so this is a historical\n  profile, not a usable auth contract. derive-authentication.py found no spec\n  files in this repo (0 auth profiles).\nsummary:\n  types:\n  - http\n  - oauth2-like\n  api_key_in: []\n  oauth2_flows:\n  - password\n  - github-browser-popup\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Long-lived Divshot access token passed to the client (`token` option) or to\n    the CLI via `-t, --token`. Obtainable from the CLI with `auth:token`.\n  sources:\n  - https://github.com/divshot/divshot-api/blob/master/README.md\n\
  \  - https://github.com/divshot/divshot-cli/blob/master/README.md\n- name: passwordGrant\n  type: oauth2\n  flow: password\n  description: >-\n    Email + password exchanged for an access token via `divshot.auth('password',\n    {email, password})`. The docs state passwords MUST NOT be stored and should\n    only come from direct user input.\n  requires_client_id: true\n  sources:\n  - https://github.com/divshot/divshot-api/blob/master/README.md\n- name: githubBrowserAuth\n  type: oauth2\n  flow: browser-popup\n  description: >-\n    Popup-based browser authentication, `divshot.auth('github')`, returning a\n    user object and an access_token without the integrator handling credentials.\n  requires_client_id: true\n  sources:\n  - https://github.com/divshot/divshot-api/blob/master/README.md\nclient_registration:\n  client_id_required: true\n  note: A client_id MUST be specified when instantiating the client.\ntoken_storage:\n  cookie: true\n  description: >-\n    `auth({store: true})`\
  \ writes an encoded access token to a cookie on the\n    current domain for one week; `authWithCookie()` re-authenticates from it.\nend_user_protection:\n  basic_auth_on_environments: >-\n    Deployed environments could be protected with HTTP basic auth via the CLI\n    (`protect` / `unprotect`) or `app.env(<env>).config({auth: 'user:pass'})`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divshot/refs/heads/main/authentication/divshot-authentication.yml
summary_line: http/oauth2-like · 3 schemes
tags:
- Company
- Web Hosting
- Static Hosting
- Front-End
- Deployment
- Developer Tools
- Defunct
- Acquired
---
